# Setting up the environment


## Install and set up Git

Git is a distributed version control system that tracks versions of files. It is often used to control source code by programmers collaboratively developing software. Git runs in the background and enables you to submit changes that automatically update the website. Note that you do not have to know anything about Git to work on this project. However, more information is available at the Wikipedia page: https://en.wikipedia.org/wiki/Git.

- Go to https://git-scm.com/downloads.
- Download and install Git.
- Immediately after installing git, set your username and password. This is what Git will use to identify your contributions. You can read about this in more detail here: https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup. Again, you don't need to know any of this in order to make contributions.
- Open a terminal.
	- Windows: Press the Windows key and then type *cmd*, *Command Prompt*, or *PowerShell*.
	- Mac: Click the Launchpad icon in the Dock, type *Terminal* in the search field, then click *Terminal*.
	- Linux: Launch the *Terminal* app.
- For both of the commands below, make sure that you replace 'Your Name' and 'youremail@example.com' with your actual name and email.
- Type `git config --global user.name "Your Name"` and press Enter.
- Type `git config --global user.email youremail@example.com` and press Enter.
- You can close the terminal now.

## Create a Github account

GitHub is a developer platform that allows developers to create, store, manage and share their code. It uses Git software, providing the distributed version control of Git plus access control, bug tracking, software feature requests, task management, continuous integration, and wikis for every project.

- Go to https://github.com/.
- Choose Sign up.
- Enter your email address and choose a password.


## Install and set up Visual Studio Code

Visual Studio Code (VS Code) is a source-code editor that includes support for debugging, syntax highlighting, intelligent code completion, snippets, code refactoring, and embedded version control with Git.

- Go to https://code.visualstudio.com/.
- Download and install Visual Studio Code.
- Open **Visual Studio Code** (VS Code) from your menu. Don't do anything here yet.
- Navigate to the [AI-in-HPE repository](https://github.com/michael-rowe/ai-in-hpe) in your browser.
- Click on the green **Clone** button, and copy the URL under the HTTPS tab.
- Go back to VS Code and choose **Clone Git repository** from the options on the Welcome page.
- Paste the URL from the VR-in-HPE repository into the field that appears at the top of VS Code.
- Choose a location to clone (i.e. copy) the files from the GitHub repository onto your computer.
- If you use Dropbox to synchronise files between computers, and you have some space available, choose Dropbox as the location for the repository.
- Install the **Markdown All in One** extension.
- The editor in VS code isn't going to look that great to start, but don't worry...we'll change that later. For now, we just want to make sure you can contribute to the project.

## Create a new file in VS code

- Go to Explorer (top left in the navigation panel).
- Create a new file by hovering over the Explorer panel of files.
- Call it your-name.md.
- Edit the file by adding some content about yourself. This will be the file you practice on.
- The default in VS Code is that files are not saved automatically, so you'll need to save your file. Press Ctrl-S to save.


## Commit your changes

In Git, a 'commit' is the change you've made to the project. This could be in the form of an edit to information in a file, renaming a file, and so on.

- Choose the Commit icon in the left-hand navigation panel (it looks like a network with nodes).
- You'll see all the changes you've made to the files in the project (remember that your changes have only been made locally on your machine...they're not part of the project yet).
- Click on the 'Commit' button at the top of the panel.
- You'll need to add a short comment that describes what it is that you've changed. This might be as simple as saying 'added new content' but may be more descriptive, depending on the nature of the change.
- Save your comment by clicking on the tick icon in the rop right.
- Sync your changes by clicking on the Sync button.


## Check that your changes have been made

It takes a couple of minutes for your updates to be converted and pushed to the Github Pages site for the project.

- Go to https://michael-rowe.github.io/ai-in-hpe//your-name to check that your new file has been correctly uploaded.
- Again, don't worry about how it looks. Once you've set up VS Code, and learned a bit of markdown, you can make it look almost any way you want.


# Optional

## Explore writing in Markdown

Markdown is a lightweight markup language for creating structured text using a plain-text editor. Markdown is widely used for blogging and instant messaging, and also used elsewhere in online forums, collaborative software, documentation pages, and readme files.

- Learn more about Markdown here: https://en.wikipedia.org/wiki/Markdown
- See this Markdown cheatsheet here: https://www.markdownguide.org/cheat-sheet/


## Install the Github mobile app

The Github mobile app enables you to edit the website from anywhere, at any time.

- Open the Play store on Android or the App Store on iOS.
- Search for 'Github' and install the app.
- Log in with the username and password you created when you set up the Github account previously.
- Check that you can browse the project files in the Github repository.