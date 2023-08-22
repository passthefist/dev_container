# Glossary of terms for this module

This document is not organized alphabetically but rather from base definitions and concepts to ones that
build off previous ones. It's reccomended to read through this in order, but for quick reference here
are the terms alphabetically:
- [Cloud Computing](#cloud-computing)
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

#### Server
In the simplest case, a server is a computer that's connected to the internet
and stores files that can be downloaded by other computers. In more complex cases servers do
things like interacting with data stored in databases and running web applications Any computer
can become a server if it's connected to other computers to share files and other information.

#### Version Control
Version Control is a general term for any software that keeps track of code changes and can
back them up on a server. Saving changes to a file doesn't keep track of previous version of
the file, and this can be useful to revert to a previous version of a file. Version Control
also helps developers work together by managing who is working what parts of a project. Each
developer can submit their changes separately, and all the changes are tracked to see who's
working on what. 

#### Code Repository

#### Git
Git is one of many version control solutions. It works by giving each

both a social network for software developers and a place for them to back
up their code. Users can share their code with others to collaborate on projects, commentin and
reviewing each other's code changes. By backing up their code, if something goes horribly wrong
on the computer they're working on, instead of losing all their work they can restore from the
backup.


#### GitHub
GitHub is both a social network for software developers and a place for them to back
up their code. Users can share their code with others to collaborate on projects, commentin and
reviewing each other's code changes. By backing up their code, if something goes horribly wrong
on the computer they're working on, instead of losing all their work they can restore from the
backup.

#### Graphical User Interface
A graphical user interface is how we generally interact with computers
through visually seeing a representation of things like files and applications on the screen. Using
a mouse to click on a folder and open it, or the touchscreen of a smartphone are examples of graphical
user interfaces. Before Graphical User Interfaces, developers interacted with computers only by
typing commands and reading text.

#### Datacenter
A datacenter is a collection of servers in one location to make managing them cheaper and easier.
Companies like Google and Facebook own their own datacenters dedicated to running their applications, but
some data centers rent servers for other companies to run their applications on. An individual might also
pay for a server in a data center to host a website or run an web application they're working on.

#### Operating System
An operating system is the group of base programs that manages computer hardware 
for programs to interact with, such as the keyboard, hard disk, RAM, and processor. It's the first
program that starts up when a computer is turned on, which then activates other programs like a 
graphical user interface for people to easily interact with the computer or the program that manages
wifi. Examples of operating systems are Windows, macOS, Android, and Linux.

#### Command Line Console
The command line console is more direct interface with the interface than the
graphical one we're used to. While the graphical inteface is easier to use, the command line console
is more powerful and allows a user to do things that the graphical interface doesn't offer.

#### Virtualization
Normally, a program runs on a computer and interacts with physical devices like a
hard disk, RAM, and processor. With virtualization, a program simulates these physical devices instead.
In this way, insted of a program running directly on a computer, it can instead run inside a program
simulating a computer. This allows for things like running Windows on a Macbook or playing an N64 game
on a laptop as if it was the game console.

#### The Cloud
The cloud usually refers to some service on the internet that expands the funcationality
of a personal computer or mobile device. A common example is storing photos in the cloud, where rather
than storing those photos on your phone they are backed up on some server that you can then access on
another computer. GitHub offers cloud storage of program code.

#### Container
In computing, a container refers to thechnology that bundles an application with all of
the other software the application needs to run, such as an operating system, third-party software libraries.
Containers are virtual environments, meaning that they can run anywhere that supports them, whether on
a personal laptop or server, without the risk of a missing software library or a different operating system
causing the application to not work.

#### Docker
Docker is one of many applications to manage and run containers. It allows easy creation
and management of containers on a personal computer.

#### Cloud Computing
Cloud Computing combines all of the above into a service that hosts appications in
the cloud. Before cloud computing, actual servers needed to be bought or rented in a datacenter. With cloud
computing, developers can instead upload containers in the same way that a cloud photo storage service
would back up photo files. These containers then run their applications as if running on an actual server,
and the developer doesn't need to worry about any of the details of the servers themselves. Making sure
a server was built correctly was a common problem before cloud computing.