## Preliminaries

Step through the instructions below to make sure that you have
everything you need to get started.

### Install git
You can download git here:
[https://git-scm.com/downloads](https://git-scm.com/downloads)

<!-- TODO: check this -->
If prompted, select the option to add the installation location to system path.

<!-- On Windows, you may need to select an option about "Adjusting your PATH environment". -->
<!-- The option "Run Git from the Windows Command Prompt" will help RStudio find git. -->

To check that the installation worked, open a terminal or command prompt:

**Windows**

* Go to the *Start* menu
* In the *Search* or *Run* line type **cmd** and press enter.

**Mac**

* Go to **Applications** -> **Utilities** -> **Terminal**

Type `git version`. You should see a short message containing some
version information.

### Configure git [](#configure)

After installing git, you need to tell it who you are. Open a terminal
window or command prompt (see above) and type the following:

```
git config --global user.email "you@youremail.com"
git config --global user.name "Your Name"
```

You can also configure git to use your preferred editor for commit
messages, e.g. on Mac:
```
git config --global core.editor nano
```

or on Windows:
```
git config --global core.editor notepad
```

It's a good idea to follow this step since the default editor selected by git is quite difficult to use!

### Sign up for an account on GitHub [](#github)

GitHub is a popular online hosting service for git repositories. It
provides a useful interface for collaboration and code sharing.

Create a free account on GitHub:

[https://github.com/join](https://github.com/join)

***If you have an academic email account you should use it here.***
GitHub users can create an unlimited number of free, public
repositories but only a limited number of private
repositories. However, academic users can request access to an
unlimited number of free private repositories.

**Optional**

If you are an academic user, sign up for free private repositories here:

[https://education.github.com/discount_requests/new](https://education.github.com/discount_requests/new)

***This requires your account to be associated with an academic email
address.***

It may take a while to receive the verification email for
this step. Don't worry, we won't need this for the tutorial.

### Install RStudio

If you're going to be following the section on using git through
RStudio, you'll need to make sure you have an up-to-date version of
RStudio installed. Downloads are available at:

[https://www.rstudio.com/products/rstudio/download/](https://www.rstudio.com/products/rstudio/download/)

#### Make sure that RStudio is ready to use git

Open Rstudio and go to the options pane (Windows users, look in
**Tools -> Options**, Mac users, look in **RStudio ->
Preferences**). The last entry in the ribbon on the left is
**Git/SVN**. Select that, and look at the contents of the box saying
**Git executable**. It should say something like `C:/Program Files
(x86)/Git/bin/git.exe` (Windows) or `/usr/bin/git` (Mac). If instead
it says `(Not found)`, RStudio cannot find git.

If RStudio cannot find git (and testing `git version` on the command
line worked above), then click the **Browse...** button and navigate
to the path corresponding to your installation of git.
