## Step 1: Planning the move

Uploading your project to GitHub gives you the feature-rich tools and collaboration needed to elevate your project to the next level. Not to mention, it's also pretty exciting. If you're doing this for the first time, you have a few options when uploading your project to GitHub. This course will guide you through the necessary steps to upload a local project to be hosted on GitHub.

### :keyboard: Activity: Exporting your project

### Your project is already on your local machine

:sparkles: Terrific! @carlonbelet since you already have the project locally, you are _almost_ ready to move it to GitHub.

To confirm: You have a project directory on your computer and you want to save it on GitHub.

**If this is correct**, close this issue to signal you are finished with this step. I will open a new issue to show you how to optimize your repository for Git operations.

## Step 2: Prepare the project

### Working with Binary files

In general, there are two types of files: text files and binary files.

Text files, like most code files, are easily tracked with Git and are very lightweight.

However, binary files like spreadsheets, presentations with slides, and videos don't work well with Git. If your repository already has some of these files, it's best to have a plan in place before you enable Git version control.

You could choose to remove the binary files, or use another tool like [git-lfs](https://git-lfs.github.com/) (Git Large File Storage). We won't get into detail on how to set up git-lfs in this course, but we will talk about `.gitignore` files next, which are key to protecting your code from becoming bloated with binaries.

### Add a `.gitignore`

To do this, you will create a file in your current project named `.gitignore`. Git will use the `.gitignore` to determine which files and directories should not be tracked under version control. The [`.gitignore` file](https://help.github.com/articles/ignoring-files/) is stored in your repository in order to share the ignore rules with any other users that interact with the repository. 

### :keyboard: Activity: Prepare your repository

  1. Remove any binary files from your repository.
  2. In your local environment, [create a `.gitignore` file](https://help.github.com/articles/ignoring-files/). You can use a [template](https://github.com/github/gitignore) or create your own.
  3. Add the following code:`# project settings for VSCode .vscode`

## Step 3: Setup connection with Github

  1. Open the integrated terminal found under View > Integrated Terminal.
  2. In your command line, type `git config --global user.name "carlonbelet"`
  3. In your command line, type `git config --global user.email "carl.onbelet@rts-consult.com"`

## Step 4: Make the move

Having a project already stored locally enables you to move it to GitHub rather quickly. The following activity provides instructions to move your local project to GitHub using various tools. Select the tool you are most comfortable with and get importing :smile:.

### Using Visual Studio Code

  1. In Visual Studio Code, open the folder for your project.
  1. Click the icon on the left for **Source Control**.
  1. On the top of the Source Control panel, click the **Git icon**.
  1. If the files you see match the repository you want to create, click **Initialize Repository**.
  1. Next to the word **CHANGES**, click the symbol of the plus sign to stage all of the changes.
        - This is part of the two stage commit. You can use this staging function to create meaningful commits throughout the development process.
  1. In the box in the Source Control panel, type a commit message. Something like "initial commit - moving project" could work.
  1. Click the checkmark at the top of the Source Control panel.
  1. Open the integrated terminal found under View > Integrated Terminal.
  1. In your command line, type `git remote add origin https://github.com/carlonbelet/github-upload`
  1. In the Source Control Panel, click the expandable three dots that open a menu of options. Or click on the blue cloud sign in the bottom left corner.
  1. When asked if you'd like to publish the branch, click **Okay**.
