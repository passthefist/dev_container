# Educational Development Environment

This repository contains the files, libraries and applications for a base development environment.

You'll set up this environment and use it to build and publish a personal website using Github's
free website hosting features. By the end, you'll be comfortable with the basic workflows around
software development and basic HTML/CSS.

There's a lot to learn here, and lots of questions to ask. What's in this document is just an overview 
and introduction. The focus is more on getting comfortable with development environments and
gaining some background on common terms and concepts in the tech world.

Refer to this page for some of the terms and concepts that will be a part of this project: [Glossary.md](Glossary.md)

## Technical Introduction ## 

Before reading through this, it's helpful to read through the glossary linked above.

You'll be installing a code editor, creating a virtual server using Docker to act as the host for your website, familliarizing yourself with version control, . 

The environment uses Docker, which is a platform that allows for easy management of virtual servers. 
It's like your own personal cloud computing environment, hosted on your computer instead of
a data center. These virtual environments are referred to as images and containers, which are
run by Docker as if they are a completely separate computer (but actually running on yours in a virtual
environment). Containers can easily be created, cloned, and updated which has a lot of advantages for software development.

By being able to create and clone servers with standard configurations, developers
can be sure they are interacting with the same environment as each other and the live environment.
Commonly, the live environment is referred to as "production" while the one 
developers work in is referred to as "development" or "local". Separating the two means that code can be tested
before it's deployed to the actual users of the application. With this setup, you'll have a development
environment using Docker and a production environment using Github's free website hosting features.

The main focus of this repository is on bulding core development practices like testing before 
deploying, using version control to keep track of code changes, and interacting with the command line 
console. A skeleton for a simple website has been provided to build these practices while also creating 
an online resume to learn basic HTML and CSS. Periodically, you'll be using Git to publish the changes
made in your local development environment to your production environment on Github.

This repository contains the files, libraries and applications for a base development environment.

The environment uses Docker, which is a platform that allows for easy management of virtual servers. 
It's like your own personal cloud computing environment, hosted on your computer instead of
some data center. These virtual environments are referred to as images and containers, which are
run by Docker as if they are a completely separate computer (but actually running on yours in a virtual
environment). Containers can easily be created, cloned, and updated which has a lot of advantages for software development.

By being able to create and clone servers with standard configurations, developers
can be sure they are interacting with the same environment as each other and the live environment.
Commonly, the live environment is referred to as "production" while the one 
developers work in is referred to as "development" or "local". Separating the two means that code can be tested
before it's deployed to the actual users of the application. With this setup, you'll have a development
environment using Docker and a production environment using Github's free website hosting features.

The main focus of this repository is on bulding core development practices like testing before 
deploying, using version control to keep track of code changes, and interacting with the command line 
console. A skeleton for a simple website has been provided to build these practices while also creating 
an online resume to learn basic HTML and CSS. Periodically, you'll be using Git to publish the changes
made in your local development environment to your production environment on Github.

## Setting Up the Environment ##

You'll need 3 things first: a code editor, Docker Desktop, and the Github application.

### 1. Code Editor ###
Download a code editor such as [https://code.visualstudio.com/download](X). Visual Studio Code is the 
preferable editor for this, but ultimately what's important is using what you're comfortable with.

### 2. Docker and Docker Desktop ###

Docker Desktop provides an interface to see and manage the containers running on your computer. 
Installing it also installs the Docker engine, which is the underlying system that provides the
virtual computing environment for the containers to run on.

Download Docker Desktop from https://www.docker.com/products/docker-desktop/
 
**Installing on Mac:**

Double-click Docker.dmg to open the installer, then drag the Docker icon to the Applications folder. You 
can then open Docker Desktop like any other app.

**Installing on Windows:**

You'll need to first install the Windows Subsystem for Linux. This provides an adaptation layer that 
mimics Linux and provides the neccesary systems for Docker to work with Windows.

To install it, open Powershell, Windows' command line console. Powershell can be opened by the start 
menu search, or hitting the (⊞ Win) + R key combination and typing "powershell" in the prompt. If you've
installed Visual Studio Code as your editor, you can go to the "Terminal" menu and choose "New Terminal"
which will open a terminal prompt in the editor.

You should see a prompt like this:

```
GitHub\dev_container>
```

Type `wsl --update` and hit enter to install the Windows Subsystem for Linux, similar to the example 
below. You should see some output that finishes with a successful update/installation or that the most
recent version is already installed.

```
GitHub\dev_container> wsl --update
```

You'll then need to log out and log back in. After logging in, you'll be able to start the Docker 
Desktop app.

### 3. Github Desktop App ###

The Github Desktop App provides an easier to use interface to Git, which is a popular solution for
keeping track of code changes. These solutions are referred to as "version control", and Git is one
of many options for version control. Since it's both the most popular and easily works with a site
like Github, it's going the be the one used here.

Developers use version control to save code in a more structured way than just saving the file as normal.
With Git, you can periodically commit your changes to keep a log of different versions of the files that
have been changed. If a bug is later discovered or a file is accidentally removed, the previous version
can be recovered (hence calling these "version control"). Git supports many features, and the Github app
makes using it easier. Different projects can have their own code repositories, allowing developers to
separate or share the code they're working on to coordinate their projects.

Download the Github Desktop app from https://desktop.github.com/. Once installed, you'll need to log in
to the app to access your Github repositories.

### 4. Clone This Repository ###

Once all the applications are installed and you've logged in to the Github app, you can clone this 
repository to download all the code to your computer. First, fork this project from the "Fork" button
in upper/middle right part of this page. It will take you to a prompt, where you can choose your user
in the top "Owner" dropdown and just keep the defaults. Clicking the "Create Fork" button will create
your own version of this project's code repository.

Then, in the upper left corner of the Github Desktop app, you can search for your repositories. Choose this one (it should be called "dev_container") to create a copy of the repository to work with locally.

You can then open the files in your code editor and use Git to commit your changes.

### 5. Start the Docker Container and Webserver ###

The easiest way to do this is opening a new terminal in Visual Studio Code from Terminal menu. You'll
see a prompt similar to this:

```
GitHub\dev_container> 
```

This is the command line console, which is a more direct and powerful interface to the operating system than the graphical desktop environment. It takes a given command on the prompt line, executing once a user hits enter. Here, we'll be using it to build and run our Docker container with the `docker-compose`
program. It has options such as `build`, `up`, and `down` to build, start, and stop containers respectively.

First, build the container by typing `docker-compose build` in the prompt and hitting enter. You should see some output similar to the line below the command.

```
GitHub\dev_container> docker-compose build

[+] Building 0.0s (0/0)
```

Then use the `docker-compose up` command to start the container and webserver. You should see some output similar to the below:

```
GitHub\dev_container> docker-compose up

[+] Running 1/0
 ✔ Container webserver  Created                                                                                     0.0s 
Attaching to webserver
webserver  | AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.18.0.2. Set the 'ServerName' directive globally to suppress this message
webserver  | AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.18.0.2. Set the 'ServerName' directive globally to suppress this message
webserver  | [Tue Aug 15 20:52:19.615725 2023] [mpm_event:notice] [pid 1:tid 139701160818560] AH00489: Apache/2.4.57 (Unix) configured -- resuming normal operations
webserver  | [Tue Aug 15 20:52:19.637751 2023] [core:notice] [pid 1:tid 139701160818560] AH00094: Command line: 'httpd -D FOREGROUND'
```

Once built, the container can be ran and managed from the Docker Desktop app.

### 6. View the Website in Your Browser ###

After the server has started, you can view the web page by visiting http://localhost/website in your
web browser. You should see an ugly website that looks like a terrible resume with fake information.

This works because your computer is running a webserver pointing to the files in this repository.
Instead of a typical url like http://google.com/search or http://www.wikipedia.com/article
which connect to the `google.com` and `www.wikipedia.com` webservers to show a "search" or "article" 
page on those servers, `localhost` refers to your own computer. Since your computer is now running a
web server, it responds by serving up the web page your browser requested.

Running Docker can take a lot of system resources like RAM and CPU. When not developing, it's best to
stop the web server conatiner, which can be done with the Docker Desktop app. Navigate to the 
Conatainers view in the sidebar menu, then find the container you want to stop. Under the actions column,
press the stop button to stop the container. The container can be restarted the same way, picking up
from the state it was in when it was stopped.

## Next Steps ##

You've now set up everything you need to build your online resume. Use your code editor to modify the
`index.html` file with content and play around with the `css/styles.css` file to change the styling
of the page. Don't worry that it's ugly or doesn't look the way you want, or you terribly break 
something. The important part is getting comfortable working in the development environment and 
commiting your changes as you go. If something is terribly broken, you can recover by going to the 
"Branch" menu in the Github app and choosing the "Discard Changes" option. This will discard all of the
changes since the most recent commit, bringing them back to a working state.

Once the development environment is set up, we'll learn the basics of HTML and CSS to change the
skeleton site into an online resume hosted with your Github account.