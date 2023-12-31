## A. WAYS TO BUILD

### Step 1: GET THE EQUIPMENT

 Installing all of the tools required to develop the website:

- [Git](https://git-scm.com/downloads): we used Git for the version control system and track of changes made to files.We used git version 2.42.0.windows.2.
- [Github](https://github.com/): For our website, we utilize the github service.
- [Github Desktop](https://desktop.github.com/):To move or push our coding from local to GitHub, we used github desktop.
- [VScode](https://code.visualstudio.com/):We used the Visual Studio code to write down our documents.
- [Nodejs](https://nodejs.org/en/):We used it to build the environment. node --version v18.18.0.
- [Markdown language](https://www.nexmaker.com/doc/1projectmanage/markdown.html): to write our document;

### Step 2: SET THE PAGE

<span> To establish a repository, visit github.com and, if necessary, create your account. Proceed to create your repository and set its visibility to Public, allowing internet users to access it. Make sure to include a README file within the repository, as this is where you can provide a comprehensive project description.
</span>

<span style=color:red>NOTE</span>
Here in the picture <span>Owner* name is Minhazul249602</span>.But When you working under an organization here should be the organization's name. For our repository <BR>
**Owner=** **NexMaker-Fab**<br>
**Repository name=** **2023zjudem-The-Dynamic-Seven**
<BR>
<img style="float: center;" width=700 src="PM/Howtobuild/github.png">
<BR>

<span>Additionally, take note of the following: To activate GitHub Pages for your repository, navigate to the repository's settings. In the "Pages" section, choose the main source branch, typically named "main," and designate the folder as "root" before saving your preferences. It's important to select the "root" folder because a "docs" folder has not yet been established for this repository. Please be aware that you may need to adjust this setting at a later time. After saving these settings, you will receive a link to your repository. Sometimes it takes some time to provide a page link.After one minute you can check the link. <br> </span> <BR>


<span style="color:red">EXAMPLE : Page </span>
<BR>
<img style="float: center;" width=700 src="PM/Howtobuild/github2.png">

### Step3: LOCAL SETTINGS
  #### 1. GitHub Desktop

<span>Launch GitHub Desktop, then clone the repository you previously created and proceed to open it in Visual Studio Code.</span>
<br>
<img style="float: center;" width=700 src="PM/Howtobuild/github_desk1.1.png">
<br>

<span>Clone with our github repository</span>
<br>
<img style="float: center;" width=700 src="PM/Howtobuild/github_desk2.png">
<br>
<br>

<span>From here we can open vs code</span>
<br>
<img style="float: center;" width=700 src="PM/Howtobuild/gd3.png">

#### 2. Vs Code
From vs code at the first open terminal for install doscsify.
<br>
<img style="float: center;" width=400 src="PM/Howtobuild/vs1.png">

#### 3. Install Docsify

To set up the environment, follow these steps:
<BR>
<span style="color:red">Method 1</span>
<BR>

1. Begin by executing the command: "npm i docsify-cli -g" to install Docsify globally.At that time some necessary file downloaded.
<br>

<br>
<img style="float: center;" width=700 src="PM/Howtobuild/doc1.png">
<br>

<BR>
2. Ensure you are in the desired directory, and then initialize the environment with the command: "docsify init ./docs."
   <br>
3. We used "docsify serve docs" command for run the server.
   <br>
<img style="float: center;" width=700 src="PM/Howtobuild/doc2.png">
<BR>
4. After running the above command, open your web browser and visit "http://localhost:3000" to access your initial website.
<BR>
<span style="color:red">Method 2</span>
<BR>

* We used a vs code extension to run our server.We used 'live Server' extension.

<br>
<img style="float: center;" width=700 src="PM/Howtobuild/live_s1.png">
<BR>
1. From vs code extension search bar search "Live Server" and Install it in vs code .
<br>
<img style="float: center;" width=700 src="PM/Howtobuild/live_s2.png">
<BR>
2. For start the server at first we have to go index.html file.Here in vs code at right down corner "Go Live" option .From here we can also run the server. <br>
   <span style="color:red;">NOTE:</span>
   <span style="color:#29fad0">Have to run server from index.html: The Entry File. </span>

<BR>
<BR>
<img style="float: center;" width=700 src="PM/Howtobuild/file.png">
<br>
   <span style="color:red">NOTE:</span> 
<span>Enter the following in command terminal: docsify init ./docs
After successful initialization, you can see several files created in the directory：
<br>index.html: Entry File.
<br>README.md: It will be rendered as the homepage content.
<br>.nojekyll: is Used to prevent GitHub Pages from ignoring files that begin with an underscore.</span>
<BR>
<span></span>


#### 4. Setting up Index.html


    <!DOCTYPE html>
    <html lang="en">
    <head>
    <meta charset="UTF-8">
    <title>The Dynamic Seven</title>
     <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
    <meta name="description" content="Description">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, minimum-scale=1.0">
    <link rel="stylesheet" href="css/bootstrap-grid.min.css"/>
    <link rel="stylesheet" href="css/fontawesome-all.min.css">
    <link rel="stylesheet" href="css/common-1.css"/>
    <link rel="stylesheet" href="css/style.css"/>
    <link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify-sidebar-collapse/dist/sidebar.min.css" />
    <meta name="theme-color" content="#ffffff">
    <link href="https://fonts.googleapis.com/css?family=Open+Sans" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/sushantrahate/docsify-darkly-theme/css/darkly.css">
  
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/sushantrahate/docsify-darkly-theme/css/darkly.min.css">
 

    <style>
    :root {
    --base-font-size                              : 14px;
    --theme-color                                 : rgb(236, 173, 35);
     }

    </style>
    </head>
    <body>
    <div id="app"></div>
    <script>
    window.$docsify = {
      name: '🌐HOME',
      repo: '',
      homepage: 'home.md',
      loadSidebar: true,                 //prepare for sidebar
      loadNavbar: true,                  //prepare for navbar
      mergeNavbar: true,
      subMaxLevel: 3,
      sidebarDisplayLevel: 1,            // set sidebar display level
    }
    </script>
    <script src="//cdn.jsdelivr.net/npm/docsify@4"></script>
    <div id="ad1_footer" style="display: none;">
    <script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script> <!-- 728-CodeLab-Demo --> <ins class="adsbygoogle"      style="display:inline-block;width:728px;height:90px"      data-ad-client="ca-pub-3311815518700050"      data-ad-slot="5805089606"></ins> <script> (adsbygoogle = window.adsbygoogle || []).push({}); </script>
    </div>
     <script src="//cdn.jsdelivr.net/npm/docsify-sidebar-collapse/dist/docsify-sidebar-collapse.min.js"></script>
     <script type="text/javascript" src="../../js/script.js"></script>
    </body>
    </html>


<span>
   - Here link up with some css files for website theme.<br>
   - Also some font link <br>
   - In this html file we set our home page.<br>
   - prepare for sidebar.<br>
   - prepare for navbar.<br>
   - set sidebar display level.<br>
</span>

#### 5.  Add sidebar and navbar

<br>
<img style="float: center;" width=400 src="PM/Howtobuild/code_sidebar.png">

<br>

- Collapsible Sidebar
to make our sidebar collapsible you just need to these things add in window.$docsify this code

       
      loadSidebar: true,                 //prepare for sidebar
      loadNavbar: true,                  //prepare for navbar
      mergeNavbar: true,
      subMaxLevel: 3,
      sidebarDisplayLevel: 1,            // set sidebar display level
    
- NAVBAR

In navagation bar we have vision ,team members information and language

<br>
<img style="float: center;" width=700 src="PM/Howtobuild/code_nav.png">

<br>

Open the Index file go to window.$docsify then add

             loadNavbar: true,

#### 6. Image Upload

We use
 We created an Image folder in docs where we stored all the pictures and we would drag and drop them into the document. using "img style="float: center;" width=700 src="url/imagename.png(format)".

 <br>
<img style="float: center;" width=700 src="PM/Howtobuild/img.png">
<BR>
<BR>
<BR>

#### 7. How to create tile,Header, and content 



-  How to add Title and Group Logo

<BR>

     <img style="display: block;
     margin-left: auto;
      margin-right: auto;
      width: 30%;" src="PM/Howtobuild/logo.png">

    <H2 style= "text-align: center; font-size:7vw" > <span style="color:green"></span><span     style="color:orange">The </span><span style="color:orange"> Dynamic Seven</span> </h2>

     <H2 style= "text-align: center; font-size:2vw" > <span style="color:light black">HELLO! <br> Welcome to The     Dynamic-Seven</span>


<BR>




- How to add Section 

<br> 

       ## A. WAYS TO BUILD
       ## B. PROBLEMS & SOLUTIONS
       ## C. SET UP TEAMINTRO
       ## D. LANGUAGE
       ## D. LANGUAGE

<BR>

- How to add subsections
<br>


       #### 1. Github Desktop
       #### 2. Vs Code
       #### 3. Install Docsify
       #### 4. Setting up Index.html
       #### 5. Add sidebar and navbar
       #### 6. Image Upload
       #### 7. How to create tile,Header, and content 


<BR>

 
- Here some codes for add text and picture .

<BR>

<span style="color:red">EXAMPLE</span>


    #### 3. Install Docsify

    To set up the environment, follow these steps:
    <BR>
    <span style="color:red">Method 1</span>
      <BR>

    1. Begin by executing the command: "npm i docsify-cli -g" to install Docsify globally.At that time some necessary         file downloaded.
      <br>

      <br>
      <img style="float: center;" width=700 src="PM/Howtobuild/doc1.png">
      <br>

    <BR>
    2. Ensure you are in the desired directory, and then initialize the environment with the command: "docsify init ./    docs."
       <br>
    3. We used "docsify serve docs" command for run the server.
       <br>
    <img style="float: center;" width=700 src="PM/Howtobuild/doc2.png">
    <BR>
    4. After running the above command, open your web browser and visit "http://localhost:3000" to access your initial     website.
    <BR>
    <span style="color:red">Method 2</span>
    <BR>

    * We used a vs code extension to run our server.We used 'live Server' extension.

    <br>
    <img style="float: center;" width=700 src="PM/Howtobuild/live_s1.png">
    <BR>
    1. From vs code extension search bar search "Live Server" and Install it in vs code .
    <br>
    <img style="float: center;" width=700 src="PM/Howtobuild/live_s2.png">
    <BR>
    2. For start the server at first we have to go index.html file.Here in vs code at right down corner "Go Live"     option .From here we can also run the server. <br>
       <span style="color:red;">NOTE:</span>
       <span style="color:#29fad0">Have to run server from index.html: The Entry File. </span>
    
    <BR>
    <BR>
    <img style="float: center;" width=700 src="PM/Howtobuild/file.png">
    <br>  
       <span style="color:red">NOTE:</span> 
    <span>Enter the following in command terminal: docsify init ./docs
    After successful initialization, you can see several files created in the directory：
    <br>index.html: Entry File.
    <br>README.md: It will be rendered as the homepage content.
    <br>.nojekyll: is Used to prevent GitHub Pages from ignoring files that begin with an underscore.</span>
    <BR>
    <span>
    </span>
......
    
<BR>

- How to add link 
<BR>


    Installing all of the tools required to develop the website:

    - [Git](https://git-scm.com/downloads):we used Git for version control system and track of changes made to files.We used git version 2.42.0.windows.2.
    - [Github](https://github.com/):For our website, we utilize the github service.
    - [Github Desktop](https://desktop.github.com/):To move or push our coding from local to github, we used github desktop.
    - [VScode](https://code.visualstudio.com/):We used the visual studio code to write down our documents.
    - [Nodejs](https://nodejs.org/en/):We used it to build the environment. node --version v18.18.0.
    - [Markdown language](https://www.nexmaker.com/doc/1projectmanage/markdown.html): to write our document;


<BR>

<BR>



### Step 4: UPLOAD Document to Github

1. Utilize GitHub Desktop to upload fresh content by switching the branch's folder from "root" to "docs."
   <br>
<br>

<img style="float: center;" width=700 src="PM/Howtobuild/git_up.png">
<BR>

1. Use GitHub Desktop to label your modifications and then commit them. For this project, we used vs code as a code editor. After updating our code we can commit and push our code, file, and images through the GitHub desktop also vs code.
   <br>
   <BR>
   <B>GitHub Desktop<BR>
<img style="float: center;" width=700 src="PM/Howtobuild/commit_1.png">
<BR>
<br>
* After editing code in vs code here we can see the changes.At first we write summary of the changes and second part write description of the changes.Third step  Click the Fetch origin button to check the GitHub repository to see if any changes have been made remotely.
<BR>
<img style="float: center;" width=700 src="PM/Howtobuild/commit_2.png">
<BR>
* Click Push origin in GitHub to send the changes in our local branch to the corresponding branch in the remote repository. Origin is the default name given to the remote repository from which our cloned your local repository.
<BR>
<BR>

<B>Push From Vs code<BR>
<BR>
<img style="float: center;" width=700 src="PM/Howtobuild/vs_push1.png">
<BR>
* After update code in vs code left side bar has source control here we can see our changed code.From here(commit & push) we can send the changes in our local branch to the corresponding branch in the remote repository.
<BR>
<BR>
<img style="float: center;" width=700 src="PM/Howtobuild/vs_push2.png">
<BR>
* Here we need to write some comments about changes in our code. And save it with "ctrl + s"..

## B. PROBLEMS & SOLUTIONS
1. At first, we faced a problem opening the page link. It happened because we chose the folder "docs" rather than choosing "root" which after saving was not giving us the webpage link.
2. Docsify init ./docs cannot be loaded because running scripts is disabled on this system.<br>

  <br>
<img style="float: center;" width=1500 src="PM/Howtobuild/prob1.png">
<BR>
   <span style="color:#17c088">Solution:</span><br>
   <span style="color:#ff5a5a">The reason why the running scripts was disable on the system was because the running mode was strict ,you can change to Unrestricted or Bypass，by using the following code: <span>Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Unrestricted -Force or Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Bypass -Force </span></span>
3. The term 'docsify' is not recognized as the name of a cmdlet, function, script file, or operable program.<br>
    <span style="color:#17c088">Solution:</span><br>
    <span style="color:#ff5a5a">This error means docsify cannot be found in the PATH. Eitherinstall it globally (recommended for many command-line tools, and where it is found in the global Github folder, already in the PATH) or run it from where it is installed in the local Github</span>

## C. SET UP TEAMINTRO

Here is some coding part How we setup our team introduction.
We upload img using this tag 
                      
        <img src="" alt=""/>

Link teammate personal portfolio  by using this code.
       
        <button class="button button1"><a href="https://minhazul249602.github.io/cv/">Personal website link</a></button>

In description part we used 
   
        <p class="description">TEAMMATE DISCRIPTION </p>

Here is the code part how we build our team introduction.

              
    <div class="demo">
    <div class="container">
    <div class="row text-center">
    <h1 class="white" style="text-align:left; font-size:40px;">MEET WITH OUR AMAZING TEAM </h1>
    <br>
    <br>
    </div>

    <div class="row">
      <div class="col-md-4 col-sm-6">
            <div class="our-team">
                <div class="pic">
                     <img src="IMAGE/profile/minhaz.png" alt=""/>
                  </div>
                   <div class="team-content">
                   <h1><a href="https://minhazul249602.github.io/cv/">MINHAZUL ISLAM</a></h1>
                            <span class="post">22351396</span><br>
                             <button class="button button1"><a href="https://minhazul249602.github.io/cv/">Personal website link</a></button>
                            <p class="description">
                              It's Minhazul Islam from Bangladesh. I'm a diligent worker and a quick learner 
                                  ,interested in technology and human behavior. I love coding and problem-solving. 
                                  I pride myself on having an open mind and trying to be really honest. I enjoy learning about people's backgrounds,tales, and travel experiences.
                            </p>
                        </div>
                    </div>
                </div>

                <div class="col-md-4 col-sm-6">
                    <div class="our-team">
                        <div class="pic">
                        <img src="IMAGE/profile/fahim.jpg" alt=""/>
                        </div>
                        <div class="team-content">
                        <h1><a href="https://fahim-rana.github.io/fahim_cv/">FAHIM RANA</a></h1>
                            <span class="post">22351418</span><br>
                             <button class="button button1"><a href="https://fahim-rana.github.io/fahim_cv/">Personal website link</a></button>
                            <p class="description">
                                 Fahim Rana is a highly motivated individual, currently dedicated to 
                                earning a Master's degree in industrial design engineering at Zhejiang 
                                University. He possesses a strong tech-savvy mindset and a deep passion for 
                                 adventure.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
                 <div class="demo">
        <div class="container">
            

                 <div class="row">
                <div class="col-md-4 col-sm-6">
                    <div class="our-team">
                        <div class="pic">
                            <img src="IMAGE/profile/afra.png" alt=""/>
                        </div>
                        <div class="team-content">
                        <h1><a href="https://afratasmim.github.io/personal-website/">TASNIM AFRA</a></h1>
                            <span class="post"> 22351383</span> <br>
                             <button class="button button1"><a href="https://afratasmim.github.io/personal-website/">Personal website link</a></button>
                            <p class="description">
                                   I am  Tasnim Afra from Bangladesh.I love programming, as well as designing,and 
                                   learning new things!I believe in taking a simplistic approach to solving problem 
                                   and also enjoy taking on challenging tasks that encourage me to think and create 
                                   outside the box and contribute to my personal growth.</p>
                        </div>
                    </div>
                </div>

                  <div class="col-md-4 col-sm-6">
                    <div class="our-team">
                        <div class="pic">
                        <img src="IMAGE/profile/sristy.jpg" alt=""/>
                        </div>
                        <BR>
                        <div class="team-content">
                        <h1><a href="https://chowdhurysristy.github.io/my_cv/">SRISTY CHOWDHURY</a></h1>
                            <span class="post">22351402</span> <br>
                             <button class="button button1"><a href="https://chowdhurysristy.github.io/my_cv/">Personal website link</a></button>
                            <p class="description">
                                I'm "Sristy Chowdhury", a motivated master's student in industrial design engineering at Zhejiang University. I am from Bangladesh. I enjoy learning new things and solving problems. You may frequently find me singing to express myself on happy or sad occasions. Join me on my imaginative and inventive journey.
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
                     <div class="demo">
        <div class="container">
            

              <div class="row">
                <div class="col-md-4 col-sm-6">
                    <div class="our-team">
                        <div class="pic">
                        <img src="IMAGE/profile/burton.jpg" alt=""/>
                        </div>
                        <div class="team-content">,
                            <h3 class="title"></h3>
                            <h1><a href="https://bkamzimbi.github.io/cv/">BURTON KAMZIMBI</a></h1>
                            <span class="post">22351385</span> <br>
                            <button class="button button1"><a href="https://bkamzimbi.github.io/cv/">Personal website link</a></button>
                            <p class="description">
                               This is Burton from Malawi studying a Master in Industrial 
                               Designing Engineering at Zhejiang University . I enjoy coding and 
                                learning latest and advanced technology. My desire  is to use my technical 
                                 skills  and experts in solving global challenges while targeting sustainable development goals.
                            </p>
                        </div>
                              </div>
                       </div>

                 <div class="col-md-4 col-sm-6">
                    <div class="our-team">
                        <div class="pic">
                            <img src="IMAGE/profile/zakir.jpg" alt=""/>
                        </div>
                        <div class="team-content">
                        <h1><a href="https://jakir669.github.io/my_cv/">JAKIR</a></h1>
                            <span class="post">22351398</span> <br>
                             <button class="button button1"><a href="https://jakir669.github.io/my_cv/">Personal website link</a></button>
                            <p class="description">
                               Hello, I'm Jakir, a dedicated Industrial Design Engineering master's
                                student at Zhejiang University. Passionate about travel, learning new skills, 
                                and nurturing innovative ideas. Aspiring to be a successful entrepreneur
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

......

## D. LANGUAGE
 Normaly our docs file look like this.It's in English Language.
<br>
<img style="float: center;" width=40% src="PM/Howtobuild/l1.png">
<BR>
Now we want to translate webpage in different languages.We like to translate website in Chinese.For that we have to create new file that consists of translated file.And that's file link up with entry file(index.html).
Here is our file structure.
<br>
<img style="float: center;" width=40% src="PM/Howtobuild/l2.png">
<BR>

STEP 1: At first we create a new file name 'CHINESE'
<br>
<img style="float: center;" width=40% src="PM/Howtobuild/lan1.png">
<BR>

STEP 2: Now we copy all the necessary files that are already translated manually.
<br>
<img style="float: center;" width=40% src="PM/Howtobuild/lan2.png">
<BR>
From navigation bar user can see our website in English and also In Chinese language.
<br>
<br>

## E. How to collaborate with team
<br>
<br>

 1. Inviting a team or person

**Step1:**  Ask for the username of the person you're inviting as a collaborator.

**Step2:** On GitHub.com, navigate to the main page of the repository as shown in the letter **labeled 1** in below figure

<br>
<img src="PM/Howtobuild/1.png" style="float: center;" width=700 >

<br>

**Step 3:** Under your repository name, click  **Settings** as shown in a letter **labeled 2** on the figure above . If you cannot see the "Settings" tab, select the  dropdown menu, then click **Settings**.

**Step 4:** In the **"Access"** section of the sidebar, click **Collaborators and teams** as displayed in letter **labeled 3.**

<br>
<img src="PM/Howtobuild/2.png" style="float: center;" width=700 >
<br>

**Step 5:** To the right of **"Manage access",** click **Add people or Add teams.**

**Step 6:** In the search field, start typing the name of the team or person to invite, then click a name in the list of matches.

<br>

<img src="PM/Howtobuild/3.png" style="float: center;" width=700>
<br>

**Step 7:** Under "Choose a role", select the repository role to grant to the team or person, then click **Add NAME to REPOSITORY**.

<img src="PM/Howtobuild/4.png" style="float: center;" width=700>

2. Removing access for a team or person

**Step1:** On GitHub.com, navigate to the main page of the repository.

**Step 2:** Under your repository name, click  **Settings**. If you cannot see the "Settings" tab, select the  dropdown menu, then click **Settings**.

**Step 3:** In the "Access" section of the sidebar, click  **Collaborators & teams.**

**Step 4:** Under "Manage access", next to the team or person whose access you'd like to remove, click **Remove.**

<br>
<img src="PM/Howtobuild/k.png" style="float: center;" width=700>
<br>

3. Filtering the list of teams and people

**Step 1:** On GitHub.com, navigate to the main page of the repository.

**Step 2:** Under your repository name, click  **Settings**. If you cannot see the "Settings" tab, select the  dropdown menu, then click **Settings.**

**Step 3:** In the "Access" section of the sidebar, click  **Collaborators & teams.**

**Step4:** Under "Manage access", in the search field, start typing the name of the team or person you'd like to find. Optionally, use the dropdown menus to filter your search.
<br>
<img src="PM/Howtobuild/k1.png" style="float: center;" width=700>
<br>

4. Changing permissions for a team or person

**Step 1:** On GitHub.com, navigate to the main page of the repository.

**Step 2:** Under your repository name, click  **Settings**. If you cannot see the "Settings" tab, select the  dropdown menu, then click **Settings**.

**Step 3:** In the "Access" section of the sidebar, click  **Collaborators & teams.**

**Step4:** Under "Manage access", next to the team or person whose role you'd like to change, select the Role dropdown menu, and click a new role.

<br>
<img src="PM/Howtobuild/k3.png" style="float: center;" width=700>
<br>
<br>

<BR>

## F. REFERENCES
 - [Nexmaker](https://www.nexmaker.com/)
 - [Docsify](https://docsify.js.org/#/?id=docsify)
 - [Jquery](http://www.bestjquery.com/)
 - [NodeJs](https://docs.npmjs.com/)
 - [Vs Code](https://code.visualstudio.com/)
 - [Vs Code Extension](https://marketplace.visualstudio.com/VSCode)
 - [HTML](https://www.w3schools.com/html/)
