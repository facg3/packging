# packging :
## What is dependancy ?  
is a file someone has written it , uesd to refer when a piece of software reiles on onther one .
 when you install programs , that rely on other progrms to works ,
these programs call dependancies .
## Why might you want to use a dependency in your project, rather than writing the code from scratch?  
so when i need dependency has written before i have to ues it , it isn't right when i written code do the same of tasks,
may this work take along of time and energy , and not as efficiency as dependancy .
but when i need dependency han not written before should i write it form scratch !
## What have traditionally been some of the issues with managing dependencies?  
1-works on longer time .  
2-may struggle to deliver something you need it .  
3-is always the risk!  
## what is package manager ?  
It is a collection of software tools thar automate the process ofr installing , upgrading , congifuring , and reomving form a operating system .
A package manager deals with packages, distributions of software and data in archive files .
## How does it help with dependencies?  
it's help me when i hava a code and i need some feature or something like tape , react packages and so on ,, it's help me!
## What is package.json ?  
it's file created when i initiate a reopstory on my project !
## what does npm init do ?  
Interactively create a package.json file 
## How do you use an installed package in your code?  
<code>npm install <pakagename> --save</code>  
 ## locally install   
command line :: npm install <package>  
…..
1.This package/module will find on your local node_modules folder and can only be usable for this project.  
2.This package/module can be accessible in using require("package") from code.  
const module = require('module');  
3.This package/module can't be accessible in command line interface
…………………
## Globally install:  
command line:: npm install <package> -g
Global modules are mostly tools like nodmon or any other module you use in your daily work  
1.This package/module will find on where node is installed in your machine , can be usable everywhere  
2.This package/module can't be accessible in using require("package") from code. 
3.This package/module can be accessible in command line interface.  
dependencies are required to run, npm install "$package"  
devDependencies only to develop , npm install "$package" –-save-dev  
## Why is it normally a bad idea to install a package globally?  
the command line tools are versioned. If your local/development machine has a different version of the tool than another machine that needs to run that tool for that project, then there could be incompatibilities.to solve it you should include your development tools in devDependencies in package.json. That way they can be versioned for each project
The first thing you need to do is remove that -g when you install modules. You should replace that with --save-dev so you can save the module as a development dependency and it will always be installed  
## 1.Where does NPM install packages? 
A package can be downloaded with the command:
npm install <package_name>
This will create the node_modules directory in your current directory (if one doesn't exist yet) and will download the package to that directory….
To confirm that npm install worked correctly, check to see that a node_modules directory exists and that it contains a directory for the package(s) you installed. You can do this by running (ls node_modules) 

## 2.Why is it important to make sure that installed packages aren't included in your repositories?    
you don't need to add the package in your repositeries and take a big space in it and these pkgs is already exist.

## 3.How do you prevent Git from including these files in your repository?  
Creat a .gitignore
https://f.top4top.net/p_696su1u11.png
From time to time, there are files you don't want Git to check in to GitHub. 
If you create a file in your repository named .gitignore, Git uses it to determine which files and directories to ignore, before you make a commit.
A .gitignore file should be committed into your repository, in order to share the ignore rules with any other users that clone the repository.
GitHub maintains an official list of recommended .gitignore files for many popular operating systems, environments, and languages in the github/gitignore public repository.
  1. In Terminal, navigate to the location of your Git repository.
  2. Enter touch .gitignore to create a .gitignore file.

