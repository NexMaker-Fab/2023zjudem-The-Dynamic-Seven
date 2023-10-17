# 1. SET UP TEAMINTRO
Get a template you would want to use [Here](http://bestjquery.com/tutorial/our-team/demo65/)

<br>
<img style="float: center;" width=700 src="IMAGE/inspect.png">


<br>
<img style="float: center;" width=700 src="IMAGE/language2.png">


# 2. LANGUAGE
normaly your docs file look like this

    .
    └── docs
       ├── README.md
       ├── index.htm
       ├── Sidebar.md
       └── navbar.md

if you want to have more languages you need creat another follder like you want make chinese so you haave have follder like China like this way.

    .
    └── docs
       ├── README.md
       ├── Home.md
       ├── index.htm
       ├── Sidebar.md
       └── navbar.md
    └── China
       ├── Home.md
       ├── README.md
       ├── index.htm
       ├── Sidebar.md
       └── navbar.md
    └── French
       ├── Home.md
       ├── index.htm
       ├── Sidebar.md
       └── navbar.md
    └── README.md   

then add in the index file

     homepage: 'home.md',
     mergeNavbar: true,

<br>
<img style="float: center;" width=700 src="IMAGE/language.png">

