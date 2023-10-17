## A. WAYS TO BUILD

### Step 1: GET THE EQUIPMENT

 Installing all of the tools required to develop the website:

- [Git](https://git-scm.com/downloads):we used Git for version control system and track of changes made to files.We used git version 2.42.0.windows.2.
- [Github](https://about.gitlab.com/):For our website, we utilize the github service.
- [Github desktop](https://www.gitbook.com/):To move or push our coding from local to github, we used github desktop.
- [VScode](https://code.visualstudio.com/):We used the visual studio code to write down our documents.
- [Nodejs](https://nodejs.org/en/):We used it to build the environment. node --version v18.18.0.
- [Markdown language](https://www.nexmaker.com/doc/1projectmanage/markdown.html): to write our document;

### Step 2: SET THE PAGE

<span> To establish a repository, visit github.com and, if necessary, create your account. Proceed to create your repository and set its visibility to Public, allowing internet users to access it. Make sure to include a README file within the repository, as this is where you can provide a comprehensive project description.
</span>

<BR>
<img style="float: center;" width=700 src="PM/Howtobuild/github.png">
<BR>

<span>Additionally, take note of the following: To activate GitHub Pages for your repository, navigate to the repository's settings. In the "Pages" section, choose the main source branch, typically named "main," and designate the folder as "root" before saving your preferences. It's important to select the "root" folder because a "docs" folder has not yet been established for this repository. Please be aware that you may need to adjust this setting at a later time. After saving these settings, you will receive a link to your repository.Some time it takes some time to provide page link.After one minute you can check the link. <br> </span> <BR>


<span style="color:red">EXAMPLE : Page </span>
<BR>
<img style="float: center;" width=700 src="PM/Howtobuild/github2.png">

### Step3: LOCAL SETTINGS
  #### 1. Github Desktop

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
From vs code at first open terminal for install doscsify.
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


<br>
<img style="float: center;" width=800 src="PM/Howtobuild/html_set.png">
<br>

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

<br>
<img style="float: center;" width=700 src="PM/Howtobuild/code_sidebar_collaps.png">

<br>
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
<br>
<img style="float: center;" width=1000 src="INTRO/NAVBAR/code_team.png">

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


## E. REFERENCES
 - [Nexmaker](https://www.nexmaker.com/)
 - [Docsify](https://docsify.js.org/#/?id=docsify)
 - [Jquery](http://www.bestjquery.com/)
 - [NodeJs](https://docs.npmjs.com/)
 - [Vs Code](https://code.visualstudio.com/)
 - [Vs Code Extension](https://marketplace.visualstudio.com/VSCode)
 - [HTML](https://www.w3schools.com/html/)