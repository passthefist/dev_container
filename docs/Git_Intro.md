# Introduction to Git and Github

See the [Glossary](docs/Glossary.md) first to get familliar with some of the terms
and concepts here.

Git and GitHub work together to provide a solution for developers to collaborate on
their work, keep track of their code, and maintain a portfolio of projects. The
difference between Git and GitHub can be confusing, since GitHub is closely tied
to Git.

GitHub is a website and application that makes using Git easier. Git is the 
[version control software](docs/Glossary.md) that is used behind the scenes of
GitHub to keep track of code. Git can be used without GitHub, but GitHub can only
be used with Git. There's other sites and applications that work with Git to do
similar things. GitHub is just one of the most popular ones, and is sort of like
a social network for software developers.

Git itself is complicated, so this just covers the basics. 

## Why Use Version Control at all?

Typically, when writing a document people periodically save what they are working.
If not, then you risk losing some of your work done since the last save should something
happen like a computer crash. But, just saving a file doesn't keep track of old versions
you might want to look at again. Online apps like Google Docs automatically save as
you go, backing it up in the cloud and keeping track of previous versions. A user can
always go back to a previous version of what they're working on, so this is an example
of simple version control. By keeping track of changes and previous versions of a
document, someone can see the history of how the document changed over time and reload
an old version if they like it better.

Software projects are much more complicated than one document, and can can have thousands
of different files with code for the project, with hundreds of developers changing
those files at the same time. Using version control helps coordinate all that work, so
developers can see the changes each other are making and maintain a history of how the
files have changed to reference if they need to. It's a more sophisticated system that's
similar to things like Google docs, where developers can download changes made by other
developers to work on together.

Even for personal projects, using version control is helpful if only to back up files
in case something would happen to lose them. It's also useful to upload projects to
sites like GitHub to create a portfolio of projects.

## An introduction to Git

To start, there's a few terms to be familliar with that you'll see around GitHub.

### Repository
A code repository is a storage location for code and other software development files. They also
store all the changes ever done to those files, and used to manage and organize a software project's 
code and collaborate with other project developers. A repository can also be thought of as a project
that's being worked on.

With GitHub, you'll have one repository on your computer and another stored in GitHub's servers.
You can download code changes from GitHub's servers to the one on your computer and upload the
changes made on your computer to be backed up on GitHub's servers.

Each developer can have their own repository on their computer, plus the shared on the server.
This lets them move code between them so they can be working on different things but still get
each other's updates when they are ready. The repository on a developer's computer can store
files that are in progress and not ready to be added to the project everyone is working on.
Once ready, the files can then be added to the project and the repository on the shared server.

The repository on a developer's computer is referred to as the "local repository" while the one
on the server is the "remote repository". Repositories are commonly reffered to as "repos" for
short.

### Origin
Since Git and GitHub work by connecting multiple different repositories for the same project,
repositories can have a name to identify them from one another. The name "origin" refers to
the repository on the shared server that holds code that has been completed and is ready to be
added to the project. For this project, your repository on the GitHub website is serving as the
origin. Origin is always a remote repository stored on a server.

### Fork
Forking a repository is creating a copy of a remote repository that's owned by someone else
to create a remote repository that's owned by you. This copies all of the code, the full history
of the project, and all of the code changes ever done in all of the files. Forks are always
done with remote repositories and create an origin repository that's owned by you.

### Clone
Cloning a repository is downloading a copy of a remote repository to create a local one on
a developer's computer. This is different from forking, where forking creates a remote repository
on a shared server instead of a developer's computer. However, it is similar to forking in how
it copies all of the code, the full history of the project, and all of the code changes ever done
in all of the files. Cloning always downloads files from an origin repository.

### Commit
Commiting adds file changes to a repository. When writing code or any document, it's good practice
to save as you go. However, when writing code it's common to be changing multiple files at once.
Sometimes the code being worked on is complicated, so it's worth keeping track of the stages of that
work in case a previous one needs to be restored or referenced.

Each commit is like a bundle of code changes that are given an identifier to be found later. If
someone discovers a bug in the code, they can go back through the commits and find the one that 
introduced the bug to better know how to fix it or restore a file to a version before that change.

Commiting is a core concept to Git and can be done many different ways, but with Github Desktop it
can easily be done by adding a message explaining what the changes are and clicking the commit
button. The red box below is where the commit message goes, the button in the green box creates
the commit, and the part to the right shows the code changes being committed.

![commiting with GitHub desktop](githubdesktop-commiting.png)

The red and green text to the right is called a diff, and shows the difference between the previous
version of the file in the repository and the new changes being committed. The left shows the old
version and the right the new one, with the parts highlighted in red and green the changes. Green
means something that was added to a file, such as the text in green on the right side saying "This
is a small change to show what a commit looks like" was added to the file, and so it's shown in green. 
Below it, the word "combines" was changed to "merges". Since
both words have an "es" at the end, that part wasn't changed. On the left, the red shows what 

As an example, if a profile image was added to a website, the commit message might be
"Added image to profile page" to track what changes were made in the commit without having to
look through the code. Even for a personal project, it's useful to keep commit messages in
case you need to refer to old work.

### Push
Pushing is how code changes are uploaded from a developer's computer and local repository to a remote
repository, usually the origin. A push may contain multiple commits, adding all the stages of
changes that a developer committed to the project at once. Pushing is only done when the code being 
worked on is ready to be added to the project and reviewed by other developers. 

### Pull/Fetch
Pulling and Fetching are how code changes are downloaded by Git from a remote repository. If another 
developer pushes theor changes to a project's origin repository, then you can get those changes on
your computer by pulling them down from the origin.

### Branch

## The GitHub Website

## The GitHub Desktop App