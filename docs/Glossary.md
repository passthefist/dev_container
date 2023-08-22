# Glossary of terms for this module

This document is not organized alphabetically but rather from base definitions and concepts to ones that
build off previous ones. It's reccomended to read through them from top to bottom, but for quick 
reference here are the terms alphabetically:
- [Cloud Computing](#cloud-computing)
- [Code Repository](#code-repository)
- [Code Editor](#code-editor)
- [Command Line Console](#command-line-console)
- [Command Line Interface (see Command Line Console)](#command-line-console)
- [Container](#container)
- [Datacenter](#datacenter)
- [Docker](#docker)
- [Git](#git)
- [Github](#github)
- [Graphical User Inter](#graphical-user-interface)
- [Operating System](#operating-system)
- [Server](#server)
- [Terminal (see Command Line Console)](#command-line-console)
- [The Cloud](#the-cloud)
- [Version Control](#version-control)
- [Virtualization](#virtualization)

### Server
In the simplest case, a server is a computer that's connected to the internet
and stores files that can be downloaded by other computers. In more complex cases servers do
things like interacting with data stored in databases and running web applications Any computer
can become a server if it's connected to other computers to share files and other information.

### Version Control
Version Control is a general term for any software that keeps track of code changes, copies of
previous versions of files, and can back them up on a server. Just saving changes to a file
like normal doesn't keep track of previous version of the file, and this can be useful to revert
to a previous version if a bug is found. Developers can upload those files to a server to be
backed up in a [Code Repository](#code-repository) in case something happens to destroy an
project files that are only stored in their computer.

Version control also helps developers work together by managing who is working what parts of a
project. Each developer can submit their changes separately, and all the changes are tracked
to see who's working on what or review those changes to make sure they are acceptable.

### Code Repository
A code repository stores a full history of all of the changes made to a project and stores all
of the files for that project. It allows a developer to restore any state of the project and
it's files, even if the changes weren't made by them. There are two types of code repositories -
local and remote. A local repository exists on a developer's computer, and keeps copies of the
files that are being worked on, but only for that developer to access. A remote repository exists
on a shared server backing up files for all developers to access.

### Git
Git is one of many version control solutions, and is the one used by GitHub. Each project using
Git gives developers a local repository to work with and shared remote one for collaberation
and backups. GitHub is a common service to provide the servers to store remote repositories.

See [Introduction to Git and Github](docs/Git_Intro.md) for more.

### GitHub
GitHub is both a social network for software developers and a place for them to back up their code. 
Users can share their code with others to collaborate on projects, commenting and reviewing
each other's code changes. By backing up their code, if something goes horribly wrong on the 
computer they're working on, instead of losing all their work they can restore from the backup.
A GitHub profile can act as a developer's portfolio showing their projects and often used to see 
their programming experience.

See [Introduction to Git and Github](docs/Git_Intro.md) for more.

### Graphical User Interface
A graphical user interface is how we generally interact with computers
through visually seeing a representation of things like files and applications on the screen. Using
a mouse to click on a folder and open it, or the touchscreen of a smartphone are examples of graphical
user interfaces. Before Graphical User Interfaces, developers interacted with computers only by
typing commands and reading text output using the [Command Line Console](#command-line-console).

### Datacenter
A datacenter is a collection of servers in one location to make managing them cheaper and easier.
Companies like Google and Facebook own their own datacenters dedicated to running their applications, but
some data centers rent servers for other companies to run their applications on. An individual might also
pay for a server in a data center to host a website or run an web application they're working on.

### Operating System
An operating system is the group of base programs that manages computer hardware 
for programs to interact with, such as the keyboard, hard disk, RAM, and processor. It's the first
program that starts up when a computer is turned on, which then activates other programs like a 
graphical user interface for people to easily interact with the computer or the program that manages
wifi. Not all programs can work on all operating systems. An application designed for Windows won't
simply run on a Mac because the two provide different ways for programs to interact with the computer.
Examples of operating systems are Windows, macOS, Android, and Linux.

### Command Line Console
The command line console is more direct interface with the interface than the graphical one we're used 
to. Instead of a visual representation using icons, folder, and a mouse or touchscreen, the command
line is text only. A user can only send text commands to the computer and read textual output of
those commands. While the graphical inteface is easier to use, the command line console is more powerful 
and allows a user to do things that can't be done using the graphical interface.

### Virtualization
Normally, a program runs on a computer and interacts with real, physical devices like a hard disk, RAM, 
and processor. With virtualization, a program simulates these physical devices instead. In this way, 
instead of a program running directly on a computer, it can instead run inside a program simulating a 
computer. This allows for things like running Windows on a Macbook or playing an N64 game
on a laptop as if it was the game console.

### The Cloud
The cloud usually refers to some service on the internet that expands the funcationality
of a personal computer or mobile device. A common example is storing photos in the cloud, where rather
than storing those photos on your phone they are backed up on some server that you can then access on
another computer. GitHub offers cloud storage of program code.

### Container
In computing, a container refers to thechnology that bundles an application with all of
the other software the application needs to run, such as an operating system, third-party software
libraries. Containers are virtual environments, meaning that they can run anywhere that supports them, 
whether on a personal laptop or server, without the risk of a missing software library or a different 
operating system causing the application to not work.

### Docker
Docker is one of many applications to manage and run containers. It allows easy creation
and management of containers on a personal computer. The Docker Desktop app is a graphical
interface to see running containers, start or stop them, and manage what they can do.

### Cloud Computing
Cloud Computing combines all of the above into a service that hosts appications in
the cloud. Before cloud computing, actual servers needed to be bought or rented in a datacenter. With 
cloud computing, developers can instead upload containers in the same way that a cloud photo storage 
service would back up photo files. These containers then run their applications as if running on an 
actual server, and the developer doesn't need to worry about any of the details of the servers 
themselves. Making sure a server was built to run programs correctly was a common problem before 
containers and cloud computing.