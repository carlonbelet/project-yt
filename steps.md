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
  1. In your command line, type `git remote add origin https://github.com/carlonbelet/github-upload` or go via the Source Control Panel, click the expandable three dots that opens a menu of options: Remote > Add remote and paste in the URL above.
  1. In the Source Control Panel, click the expandable three dots that open a menu of options: Branch > Publish Branche. Or click on the blue cloud sign in the bottom left corner.
  1. When asked if you'd like to publish the branch, click **Okay**.

## Step 5: Private or Public?

Right now, your repository is set to public.

You can change the visibility of a repository to Private or Public at any time in your repository's **Settings** tab, but there are some things you should know.

### Private Repositories
If your repository is private, the only people who can see your code are you and the collaborators <sup>[:book:](https://help.github.com/articles/github-glossary/#collaborator)</sup> you've invited.

### Public Repositories
In public repositories, anybody can see your code. Millions of open source repositories on GitHub are public, too!

Licenses, code of conduct, and other files are important when you create a public repository. There are many benefits to this, but it's also a large responsibility. Keep in mind that once a repository is public _and_ open source, there are certain implications about keeping it public, depending on the license chosen.

> It's important to note that public does **not** equal open source! The license associated with code determines whether or not it is open source.

## Step 6: Create a beta release

Create a release for this repository on GitHub.

GitHub Releases point to a specific commit. Releases can include release notes in Markdown, and attached binaries.

Before using a release based workflow for a larger release, let's create a tag and release.

### :keyboard: Activity: Create a release for the current codebase

1. Go to the [**Releases** page](https://github.com/carlonbelet/release-based-workflow/releases) for this repository.
    - You can click the link above, or click the **Code** tab at the top of your repository. Then, find the navigation bar below the repository description, and click **0 releases**.
1. Click **Create a new release**.
1. In the field for _Tag version_, specify a number. In this case, use **v0.9**. Keep the _Target_ as **main**.
1. Give the release a title, like "First beta release". If you'd like, you could also give the release a short description.
1. Select the checkbox next to **This is a pre-release**, since it is representing a beta version.
1. Click **Publish release**.

Op dit moment wordt er wel een tag aangemaakt en een release. De code basis wordt meegenomen in een zip bestand.

## Step 7: Create a project board

### Organizing Releases

Creating a release package on GitHub might be easy, but it's only a piece of the puzzle. Releases often involve prioritized bug fixes, feature releases, and assorted tasks. How do you make sure you're keeping track? What happens if you want to save the most exciting features for a larger update?

On GitHub, let's keep track of several related issues with a GitHub project board.

### :keyboard: Activity: Create a project board

1. Navigate to the [Projects](https://github.com/carlonbelet/release-based-workflow/projects) tab of this repository.
1. Click **Create a project**.
1. Under **Project board name**, type "Release 1.0 tracker".
1. In the **Template** dropdown, select **Automated kanban**.
1. Click **Create project**.
