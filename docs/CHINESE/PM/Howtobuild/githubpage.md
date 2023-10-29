
## A. 构建方法


### 第 1 步：获取设备

 
安装开发网站所需的所有工具：

- [Git](https://git-scm.com/downloads):
我们使用 Git 作为版本控制系统并跟踪对文件所做的更改。我们使用 git 版本 2.42.0.windows.2。
- [Github](https://github.com/): 
对于我们的网站，我们使用 GitHub 服务。
- [Github desktop](https://desktop.github.com/):
为了将我们的代码从本地移动或推送到 Github，我们使用 GitHub 桌面。
- [VScode](https://code.visualstudio.com/):
我们使用 Visual Studio 代码来写下我们的文档。
- [Nodejs](https://nodejs.org/en/):
我们用它来构建环境。节点--版本 v18.18.0。
- [Markdown language](https://www.nexmaker.com/doc/1projectmanage/markdown.html): 
撰写我们的文件；


### 第 2 步：设置页面
<span> 
要建立存储库，请访问 github.com，并根据需要创建您的帐户。继续创建您的存储库并将其可见性设置为公共，以允许互联网用户访问它。确保在存储库中包含自述文件，因为您可以在其中提供全面的项目描述
</span>
<br>
<img style="float: center;" width=700 src="PM/Howtobuild/github.png">
<BR>

<span>
此外，请注意以下事项： 要为您的存储库激活 GitHub Pages，请导航到存储库的设置。在“页面”部分中，选择主要源分支（通常名为“main”），并在保存首选项之前将该文件夹指定为“根”。选择“root”文件夹很重要，因为尚未为此存储库建立“docs”文件夹。请注意，您稍后可能需要调整此设置。保存这些设置后，您将收到存储库的链接。有时提供页面链接需要一些时间。一分钟后您可以检查链接。
<br> </span> <BR>

<span style="color:red">EXAMPLE 例子: Page </span>
<BR>
<img style="float: center;" width=700 src="PM/Howtobuild/github2.png">

### 第 3 步：本地设置

  #### 1. Github Desktop

<span>
启动 GitHub Desktop，然后克隆之前创建的存储库并继续在 Visual Studio Code 中打开它。
</span>
<br>
<img style="float: center;" width=700 src="PM/Howtobuild/github_desk1.1.png">
<br>

<span>
使用我们的 GitHub 存储库进行克隆
</span>
<br>
<img style="float: center;" width=700 src="PM/Howtobuild/github_desk2.png">
<br>
<br>

<span>
从这里我们可以打开vs code
</span>
<br>
<img style="float: center;" width=700 src="PM/Howtobuild/gd3.png">

#### 2. Vs Code

首先从 vs code 打开终端来安装doscsify。
<br>
<img style="float: center;" width=700 src="PM/Howtobuild/vs1.png">

#### 3.安装文档化

若要设置环境，请执行以下步骤：

<BR>
<span style="color:red">方法1</span>
<BR>
1. 首先执行命令: "npm i docsify-cli -g" to install Docsify globally. 全局安装 Docsify。当时下载了一些必要的文件。
<br>

<br>
<img style="float: center;" width=700 src="PM/Howtobuild/doc1.png">
<br>

<BR>
2. 确保您位于所需的目录中，然后使用以下命令初始化环境："docsify init ./docs."
   <br>
3. 我们使用“docsifyserve docs”命令来运行服务器。
   <br>
<img style="float: center;" width=700 src="PM/Howtobuild/doc2.png">
<BR>
4. 运行上述命令后，打开 Web 浏览器并访问 http://localhost:3000 以访问您的初始网站。
<BR>
<span style="color:red">方法2</span>
<BR>

* 我们使用VS代码扩展程序来运行服务器。我们使用的“ Live Server”扩展名。

<br>
<img style="float: center;" width=700 src="PM/Howtobuild/live_s1.png">
<BR>
1. 从VS代码扩展搜索栏搜索“ Live Server”，然后将其安装在VS代码中。
<br>
<img style="float: center;" width=700 src="PM/Howtobuild/live_s2.png">
<BR>
2. 为了首先启动服务器，我们必须转到index.html文件。在vs code的右下角“Go Live”选项中。从这里我们也可以运行服务器. <br>
   <span style="color:red;">笔记：</span>
   <span style="color:#29fad0">必须从index.html运行服务器：条目文件。 </span>

<BR>
   <br>
<img style="float: center;" width=700 src="PM/Howtobuild/file.png">
<br>
   <span style="color:red">NOTE:</span> 
<span> 在命令终端中输入以下内容: docsify init ./docs

初始化成功后，可以看到目录下创建了几个文件：
<br>index.html: 入口文件.
<br>README.md: 将渲染为首页内容。
<br>.nojekyll: 用于防止 GitHub Pages 忽略以下划线开头的文件
</span>

#### 4. 建立Index.html

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


 * 这里链接一些网站主题的 css 文件。<br>
 * 还有一些字体链接<br>
 * 在这个html文件中我们设置我们的主页。<br>
 * 准备侧边栏。<br>
 * 准备导航栏。<br>
 * 设置侧边栏显示级别。<br>


#### 5.添加侧边栏和导航栏

<br>
<img style="float: center;" width=400 src="PM/Howtobuild/code_sidebar.png">

<br>

 - 可折叠侧边栏
要使我们的侧边栏可折叠，您只需要将这些东西添加到窗口中即可。.$docsify this code

      loadSidebar: true,                 //prepare for sidebar
      loadNavbar: true,                  //prepare for navbar
      mergeNavbar: true,
      subMaxLevel: 3,
      sidebarDisplayLevel: 1,            // set sidebar display level

<BR>

- NAVBAR
导航栏中有愿景、团队成员信息和语言

<br>
<img style="float: center;" width=500 src="PM/Howtobuild/code_nav.png">
<br>

打开索引文件转到窗口.$docsify然后添加:

             loadNavbar: true,

#### 6. 图像上传

 我们用
 我们在文档中创建了一个图像文件夹，其中存储了所有图片，并将它们拖放到文档中。"img style="float: center;" width=700 src="url/imagename.png(format)".

 <br>
<img style="float: center;" width=700 src="PM/Howtobuild/img.png">
<BR>


#### 7. 如何创建瓷砖，标题和内容



-  如何添加标题和组徽标

<BR>

     <img style="display: block;
     margin-left: auto;
      margin-right: auto;
      width: 30%;" src="PM/Howtobuild/logo.png">

    <H2 style= "text-align: center; font-size:7vw" > <span style="color:green"></span><span     style="color:orange">The </span><span style="color:orange"> Dynamic Seven</span> </h2>

     <H2 style= "text-align: center; font-size:2vw" > <span style="color:light black">HELLO! <br> Welcome to The     Dynamic-Seven</span>


<BR>




 - 如何添加部分

<br> 

       ## A. WAYS TO BUILD
       ## B. PROBLEMS & SOLUTIONS
       ## C. SET UP TEAMINTRO
       ## D. LANGUAGE
       ## D. LANGUAGE

<BR>

 - 如何添加小节
<br>


       #### 1. Github Desktop
       #### 2. Vs Code
       #### 3. Install Docsify
       #### 4. Setting up Index.html
       #### 5. Add sidebar and navbar
       #### 6. Image Upload
       #### 7. How to create tile,Header, and content 


<BR>

 
 - 添加文本和图片的一些代码。

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
    
<BR>

 - 如何添加链接
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
<BR>
<BR>

### 第 4 步：将文档上传到 Github

1. 利用 GitHub Desktop 通过将分支的文件夹从“根”切换到“文档”来上传新内容。
   <br>
<br>

<img style="float: center;" width=700 src="CHINESE/PM/Howtobuild/git_up.png">
<BR>

1. 使用 GitHub Desktop 标记您的修改，然后提交它们。对于这个项目，我们使用 vs code 作为代码编辑器。更新代码后，我们可以通过 GitHub 桌面提交和推送我们的代码、文件和图像，也可以与代码相比。
   <br>
   <BR>
   <B>GitHub Desktop<BR>
<img style="float: center;" width=700 src="CHINESE/PM/Howtobuild/commit_1.png">
<BR>
<br>
* 在此处编辑 vs 代码中的代码后，我们可以看到更改。首先，我们写一个更改的摘要，第二部分写一个更改的描述。第三步 单击“获取源”按钮以检查 GitHub 存储库以查看是否进行了任何远程更改。
<BR>
<img style="float: center;" width=700 src="CHINESE/PM/Howtobuild/commit_2.png">
<BR>
* 在 GitHub 中单击推送源，将本地分支中的更改发送到远程仓库中的相应分支。Origin 是我们从中克隆本地存储库的远程存储库的默认名称。
<BR>
<BR>

<B>Push From Vs code<BR>
<BR>
<img style="float: center;" width=700 src="CHINESE/PM/Howtobuild/vs_push1.png">
<BR>
* 更新 vs 代码左侧栏中的代码后，这里有源代码控制，我们可以看到我们更改的代码。从这里（提交和推送），我们可以将本地分支中的更改发送到远程仓库中的相应分支。
<BR>
<BR>
<img style="float: center;" width=700 src="CHINESE/PM/Howtobuild/vs_push2.png">
<BR>
* 在这里，我们需要写一些关于代码更改的注释。并使用“ctrl + s”保存它。

## B. 问题与解决方案
1.	起初，我们在打开页面链接时遇到了问题。发生这种情况是因为选择文件夹“docs”而不是选择“root”，保存后并没有给我们网页链接。
2.	Docsify init ./docs 无法加载，因为在此系统上禁用运行脚本。<br>
   <span style="color:#17c088">Solution:</span><br>
   <span style="color:#ff5a5a">系统上禁用运行脚本的原因是因为运行模式严格，您可以使用以下代码更改为无限制或绕过： Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Unrestricted -Force or Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Bypass -Force</span>

3. 术语“docsify”不被识别为 cmdlet、函数、脚本文件或可操作程序的名称.<br>
     <br>
<img style="float: center;" width=1500 src="CHINESE/PM/Howtobuild/prob1.png">
<BR>
<span style="color:#17c088">Solution:</span><br>
<span style="color:#ff5a5a">
此错误意味着在 PATH 中找不到 docsify。要么全局安装（推荐用于许多命令行工具，并且可以在全局 Github 文件夹中找到它，已经在 PATH 中），要么从本地 GitHub 中安装的位置运行它
</span>

## C. 设置

这是我们如何设置团队介绍的一些编码部分。
我们使用此标签上传图像

        <img src="" alt=""/>

通过使用此代码链接队友个人投资组合。

        <button class="button button1"><a href="https://minhazul249602.github.io/cv/">Personal website link</a></button>

在说明部分中我们使用了

        <p class="description">TEAMMATE DISCRIPTION </p>

这是我们建立团队介绍的代码部分。

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


## D. 语言

 通常，您的文档文件看起来像这样。用英语。
<br>
<img style="float: center;" width=40% src="PM/Howtobuild/l1.png">
<BR>
现在，我们想用不同的语言翻译网页。我们想在中文中翻译网站。为此，我们必须创建由翻译文件组成的新文件。该文件与输入文件（index.html）一起链接。
这是我们的文件结构。
<br>
<img style="float: center;" width=40% src="PM/Howtobuild/l2.png">
<BR>

步骤1：首先，我们创建一个新的文件名“中文”
<br>
<img style="float: center;" width=40% src="PM/Howtobuild/lan1.png">
<BR>

步骤2：现在，我们复制已经手动翻译的所有必要文件。
<br>
<img style="float: center;" width=40% src="PM/Howtobuild/lan2.png">
<BR>

从导航栏中的用户可以用英语和中文查看我们的网站。


## E. How to collaborate with team

## D. 引用
 - [Nexmaker](https://www.nexmaker.com/)
 - [Docsify](https://docsify.js.org/#/?id=docsify)
 - [Jquery](http://www.bestjquery.com/)
 - [NodeJs](https://docs.npmjs.com/)
 - [Vs Code](https://code.visualstudio.com/)
 - [Vs Code Extension](https://marketplace.visualstudio.com/VSCode)
 - [HTML](https://www.w3schools.com/html/)