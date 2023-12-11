## Processing
Processing is a flexible software sketchbook and a language for learning how to code. Since 2001, Processing has promoted software literacy within the visual arts and visual literacy within technology. There are tens of thousands of students, artists, designers, researchers, and hobbyists who use Processing for learning and prototyping.
## Download Software
[Download Processing](https://processing.org/download/)


## Processing and Keyboard  Interaction
This example combines  keyboard input with moving shapes a cross the screen.

<video width="720" height="500" controls>
<source src="PM/IPA/game/keyboard.mp4" type="video/mp4">
<source src="PM/IPA/game/Keyboard.ogg" type="video/ogg">
</video>

```
//move a shape around the screen according to keyboard inputs
int x=100;   //declare x and y coordinates  of the ellipse
int y=100;

void setup(){
  size(640, 480);
  pixelDensity(2);
  stroke(0);
  ellipse(x,y,10,10);
}

void draw(){
  //stroke(0);
  //ellipse(x,y,10,10);
  
  if ((keyPressed == true) && (key == 'u' || key == 'U')){
    stroke(255,0,0);
    y--;
  }
  else if (keyPressed == true && (key == 'd' || key =='D')){
    stroke(0,255,0);
    y++;
  }
  else if (keyPressed == true && (key == 'r' || key == 'R')){
    stroke(0,0,255);
    x++;
  }
  else if (keyPressed == true && (key == 'l' || key == 'L')){
    stroke(255,255,0);
    x--;
  }
  else {
    ellipse(x,y,10,10);
  }
}

```
<br>

The beginning position is just a black circle drawn to the middle of the display window. It doesn't do anything unless you type the u, d, l, or r keys, in which case the circle jumps up, down, left, or right, and changes color. If no key is being pressed, the circle just sits still in its most recent position with its most recent color.
<br>

## Description of the functions used in the above example
<br>

[Size()](https://processing.org/reference/size_.html)
* It defines the dimension of the display window width and height in units of pixels. 
* Program that has the setup() function, the size() function must be the first line of code inside setup(), and the setup() function must appear in the code tab with the same name as your sketch folder.
* The built-in variables width and height are set by the parameters passed to this function.
* For example, running size(640, 480) will assign 640 to the width variable and 480 to the height variable. If size() is not used, the window will be given a default size of 100 x 100 pixels.
<br>

[pixelDensity()](https://processing.org/reference/pixelDensity_.html)
<br>

* It makes it possible for Processing to render using all the pixels on high resolutions screens.
* This function can only be run once within a program, and must be called right after size() in a program without a setup() function, or within setup() if present.
* PixelDensity() should only be used with hardcoded numbers (in almost all cases this number will be 2)
  <br>
[Stroke()](https://processing.org/reference/stroke_.html)
<br>

* Sets the color used to draw lines and borders around shapes.
*  This color is either specified in terms of the RGB or HSB color depending on the current colorMode(). 
* The default color space is RGB, with each value in the range from 0 to 255.
<br>

[ellipse()](https://processing.org/reference/ellipse_.html)
<br>
* Draws an ellipse (oval) to the screen. An ellipse with equal width and height is a circle.
* By default, the first two parameters set the location, and the third and fourth parameters set the shape's width and height.
* The origin may be changed with the ellipseMode() function.
<br>

[keyPressed()](https://processing.org/reference/keyPressed_.html)

<br>

* The keyPressed() function is called once every time a key is pressed. The key that was pressed is stored in the key variable.
  
<br>

## Processing and Mouse Interaction
<br>
This is a simple program that demonstrate how the mouse interact with the processing
<br>

<video width="720" height="500" controls>
<source src="PM/IPA/game/mouse.mp4" type="video/mp4">
<source src="PM/IPA/game/mouse.ogg" type="video/ogg">
</video>

<br>

```
color value= color(255,0,0);
color value2= color(0,255,0);
 void setup(){
     size(200,200);
   background(255);
 }
   //click within the square to change the color of the other square
 void draw(){
   fill(value);
   rect(25,25,50,50);
   fill(value2);
   rect(75,75,50,50);
 }
 //the mouse clicked function is called after  a mouse button is pressed and then released.
 void mouseClicked() {
   //if the cursor is inside the top square and  the color of the bottom square is green
   if(mouseX<75 && mouseY<75 && mouseX>25 && mouseY>25 && value2==color(0,255,0)){
     value2=color(0,255,255);
   }
   //if the cursor is inside the top square and  the color of the bottom square is aqua
    
    else if(mouseX<75 && mouseY<75 && mouseX>25 && mouseY>25 && value2==color(0,255,255)){
     value2=color(0,255,0);
    }
    //if the cursor is inside the top square and  the color of the top square is red
   
    else if (mouseX<125 && mouseY<125 && mouseX>75 && mouseY>75 && value==color(255,0,0)){
     value=color(255, 0,255);
    
    } 
     //if the cursor is inside the bottom square and  the color of the top square is pink 
     else if (mouseX<125 && mouseY<125 && mouseX>75 && mouseY>75 && value==color(255,0,255)){
     value=color(255, 0,0);
     }
     //tell me if i haven't satisfied any of the above  possibilities
     else{
       println( "you have to click inside a square  for something to happens");
   }
 }
 ```
 <br>

## Using processing to create a game
This game is  called a flappy pong which is a sort of a combination of Flappy Bird, Pong and Brick Breaker.
<br>

<video width="720" height="500" controls>
<source src="PM/IPA/game/game.mp4" type="video/mp4">
<source src="PM/IPA/game/game.ogg" type="video/ogg">
</video>

<br>

```
********* VARIABLES *********/
// We control which screen is active by settings / updating
// gameScreen variable. We display the correct screen according
// to the value of this variable.
// 
// 0: Initial Screen
// 1: Game Screen
// 2: Game-over Screen 

int gameScreen = 0;

// gameplay settings
float gravity = .3;
float airfriction = 0.00001;
float friction = 0.1;

// scoring
int score = 0;
int maxHealth = 100;
float health = 100;
float healthDecrease = 1;
int healthBarWidth = 60;

// ball settings
float ballX, ballY;
float ballSpeedVert = 0;
float ballSpeedHorizon = 0;
float ballSize = 20;
color ballColor = color(0);

// racket settings
color racketColor = color(0);
float racketWidth = 100;
float racketHeight = 10;

// wall settings
int wallSpeed = 5;
int wallInterval = 1000;
float lastAddTime = 0;
int minGapHeight = 200;
int maxGapHeight = 300;
int wallWidth = 80;
color wallColors = color(44, 62, 80);
// This arraylist stores data of the gaps between the walls. Actuals walls are drawn accordingly.
// [gapWallX, gapWallY, gapWallWidth, gapWallHeight, scored]
ArrayList<int[]> walls = new ArrayList<int[]>();

/********* SETUP BLOCK *********/

void setup() {
  size(500, 500);
  // set the initial coordinates of the ball
  ballX=width/4;
  ballY=height/5;
  smooth();
}


/********* DRAW BLOCK *********/

void draw() {
  // Display the contents of the current screen
  if (gameScreen == 0) { 
    initScreen();
  } else if (gameScreen == 1) { 
    gameScreen();
  } else if (gameScreen == 2) { 
    gameOverScreen();
  }
}


/********* SCREEN CONTENTS *********/

void initScreen() {
  background(236, 240, 241);
  textAlign(CENTER);
  fill(52, 73, 94);
  textSize(70);
  text("Flappy Pong", width/2, height/2);
  textSize(15); 
  text("Click to start", width/2, height-30);
}
void gameScreen() {
  background(236, 240, 241);
  drawRacket();
  watchRacketBounce();
  drawBall();
  applyGravity();
  applyHorizontalSpeed();
  keepInScreen();
  drawHealthBar();
  printScore();
  wallAdder();
  wallHandler();
}
void gameOverScreen() {
  background(44, 62, 80);
  textAlign(CENTER);
  fill(236, 240, 241);
  textSize(12);
  text("Your Score", width/2, height/2 - 120);
  textSize(130);
  text(score, width/2, height/2);
  textSize(15);
  text("Click to Restart", width/2, height-30);
}


/********* INPUTS *********/

public void mousePressed() {
  // if we are on the initial screen when clicked, start the game 
  if (gameScreen==0) { 
    startGame();
  }
  if (gameScreen==2) {
    restart();
  }
}



/********* OTHER FUNCTIONS *********/

// This method sets the necessary variables to start the game  
void startGame() {
  gameScreen=1;
}
void gameOver() {
  gameScreen=2;
}

void restart() {
  score = 0;
  health = maxHealth;
  ballX=width/4;
  ballY=height/5;
  lastAddTime = 0;
  walls.clear();
  gameScreen = 1;
}

void drawBall() {
  fill(ballColor);
  ellipse(ballX, ballY, ballSize, ballSize);
}
void drawRacket() {
  fill(racketColor);
  rectMode(CENTER);
  rect(mouseX, mouseY, racketWidth, racketHeight, 5);
}

void wallAdder() {
  if (millis()-lastAddTime > wallInterval) {
    int randHeight = round(random(minGapHeight, maxGapHeight));
    int randY = round(random(0, height-randHeight));
    // {gapWallX, gapWallY, gapWallWidth, gapWallHeight, scored}
    int[] randWall = {width, randY, wallWidth, randHeight, 0}; 
    walls.add(randWall);
    lastAddTime = millis();
  }
}
void wallHandler() {
  for (int i = 0; i < walls.size(); i++) {
    wallRemover(i);
    wallMover(i);
    wallDrawer(i);
    watchWallCollision(i);
  }
}
void wallDrawer(int index) {
  int[] wall = walls.get(index);
  // get gap wall settings 
  int gapWallX = wall[0];
  int gapWallY = wall[1];
  int gapWallWidth = wall[2];
  int gapWallHeight = wall[3];
  // draw actual walls
  rectMode(CORNER);
  noStroke();
  strokeCap(ROUND);
  fill(wallColors);
  rect(gapWallX, 0, gapWallWidth, gapWallY, 0, 0, 15, 15);
  rect(gapWallX, gapWallY+gapWallHeight, gapWallWidth, height-(gapWallY+gapWallHeight), 15, 15, 0, 0);
}
void wallMover(int index) {
  int[] wall = walls.get(index);
  wall[0] -= wallSpeed;
}
void wallRemover(int index) {
  int[] wall = walls.get(index);
  if (wall[0]+wall[2] <= 0) {
    walls.remove(index);
  }
}

void watchWallCollision(int index) {
  int[] wall = walls.get(index);
  // get gap wall settings 
  int gapWallX = wall[0];
  int gapWallY = wall[1];
  int gapWallWidth = wall[2];
  int gapWallHeight = wall[3];
  int wallScored = wall[4];
  int wallTopX = gapWallX;
  int wallTopY = 0;
  int wallTopWidth = gapWallWidth;
  int wallTopHeight = gapWallY;
  int wallBottomX = gapWallX;
  int wallBottomY = gapWallY+gapWallHeight;
  int wallBottomWidth = gapWallWidth;
  int wallBottomHeight = height-(gapWallY+gapWallHeight);

  if (
    (ballX+(ballSize/2)>wallTopX) &&
    (ballX-(ballSize/2)<wallTopX+wallTopWidth) &&
    (ballY+(ballSize/2)>wallTopY) &&
    (ballY-(ballSize/2)<wallTopY+wallTopHeight)
    ) {
    decreaseHealth();
  }
  if (
    (ballX+(ballSize/2)>wallBottomX) &&
    (ballX-(ballSize/2)<wallBottomX+wallBottomWidth) &&
    (ballY+(ballSize/2)>wallBottomY) &&
    (ballY-(ballSize/2)<wallBottomY+wallBottomHeight)
    ) {
    decreaseHealth();
  }

  if (ballX > gapWallX+(gapWallWidth/2) && wallScored==0) {
    wallScored=1;
    wall[4]=1;
    score();
  }
}

void drawHealthBar() {
  noStroke();
  fill(189, 195, 199);
  rectMode(CORNER);
  rect(ballX-(healthBarWidth/2), ballY - 30, healthBarWidth, 5);
  if (health > 60) {
    fill(46, 204, 113);
  } else if (health > 30) {
    fill(230, 126, 34);
  } else {
    fill(231, 76, 60);
  }
  rectMode(CORNER);
  rect(ballX-(healthBarWidth/2), ballY - 30, healthBarWidth*(health/maxHealth), 5);
}
void decreaseHealth() {
  health -= healthDecrease;
  if (health <= 0) {
    gameOver();
  }
}
void score() {
  score++;
}
void printScore() {
  textAlign(CENTER);
  fill(0);
  textSize(30); 
  text(score, height/2, 50);
}

void watchRacketBounce() {
  float overhead = mouseY - pmouseY;
  if ((ballX+(ballSize/2) > mouseX-(racketWidth/2)) && (ballX-(ballSize/2) < mouseX+(racketWidth/2))) {
    if (dist(ballX, ballY, ballX, mouseY)<=(ballSize/2)+abs(overhead)) {
      makeBounceBottom(mouseY);
      ballSpeedHorizon = (ballX - mouseX)/10;
      // racket moving up
      if (overhead<0) {
        ballY+=(overhead/2);
        ballSpeedVert+=(overhead/2);
      }
    }
  }
}
void applyGravity() {
  ballSpeedVert += gravity;
  ballY += ballSpeedVert;
  ballSpeedVert -= (ballSpeedVert * airfriction);
}
void applyHorizontalSpeed() {
  ballX += ballSpeedHorizon;
  ballSpeedHorizon -= (ballSpeedHorizon * airfriction);
}
// ball falls and hits the floor (or other surface) 
void makeBounceBottom(float surface) {
  ballY = surface-(ballSize/2);
  ballSpeedVert*=-1;
  ballSpeedVert -= (ballSpeedVert * friction);
}
// ball rises and hits the ceiling (or other surface)
void makeBounceTop(float surface) {
  ballY = surface+(ballSize/2);
  ballSpeedVert*=-1;
  ballSpeedVert -= (ballSpeedVert * friction);
}
// ball hits object from left side
void makeBounceLeft(float surface) {
  ballX = surface+(ballSize/2);
  ballSpeedHorizon*=-1;
  ballSpeedHorizon -= (ballSpeedHorizon * friction);
}
// ball hits object from right side
void makeBounceRight(float surface) {
  ballX = surface-(ballSize/2);
  ballSpeedHorizon*=-1;
  ballSpeedHorizon -= (ballSpeedHorizon * friction);
}
// keep ball in the screen
void keepInScreen() {
  // ball hits floor
  if (ballY+(ballSize/2) > height) { 
    makeBounceBottom(height);
  }
  // ball hits ceiling
  if (ballY-(ballSize/2) < 0) {
    makeBounceTop(0);
  }
  // ball hits left of the screen
  if (ballX-(ballSize/2) < 0) {
    makeBounceLeft(0);
  }
  // ball hits right of the screen
  if (ballX+(ballSize/2) > width) {
    makeBounceRight(width);
  }
}
```

## Reference
[processing](http://www.processing.org/)
[keyboard interaction](https://www.e-education.psu.edu/earth801/node/555)
[Game](https://www.toptal.com/game/ultimate-guide-to-processing-simple-game)

