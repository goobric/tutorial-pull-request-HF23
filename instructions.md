## Here are instructions on how to: Fork, make New Branch, Clone, flag Issue, Make Changes, and Pull Request.

- [Star](#star)
- [Fork](#fork)
- [New Branch](#new-branch)
- [Clone](#clone)
- [Flag Issues](#flag-issues)
- [Make Changes](#make-changes)
- [Pull Request](#pull-request)

### Star

When you 'star' a repository, this is giving the project a thumbs-up / like.
![like the project](images/01starrepo.png)

### Fork

'forking' is a term used in github to copy a repository of a project and store it in your github account.

1. Click on the Fork button in the top right of the page, under the main title.

   ![initial Fork](images/02forkrepo1.png)

1. This will open a new window with your github account followed by the repository you are copying. Click the green Create fork button to copy this repository into your github account.
   ![copy Fork](images/02forkrepo2.png)

1. A window will open with your github account showing the repository you have just copied. Under the title of the repository, it will state 'forked from' with the name of the project owner, and the name of the repository.
   ![your Fork](images/02forkrepo3.png)

### New Branch

github uses the Tree as a visual analogy of file management, and file changes.

1. Making a 'new branch' means copying all the files and folders from the main repository, into a separate branch. This keeps the main branch in its original state, without any accidental changes.

1. In your github account, with the 'forked' (copied) repository, click the 'main' button underneath the repository title.
   ![new branch](images/04newbranch1.png)
   Give the new branch a descriptive name

1. **IMPORTANT:** next click on 'Create branch:(name) from main' this copies all the files from the main branch.
   ![use new branch](images/04newbranch2.png)

### Clone

'cloning' is a term used in github to copy a repository to your computer, creating a copy of the folders and files on the hard drive of your computer.

1. Click the green Code button a dropdown menu will appear. Click on the icon with the two squares next to the url to copy it.

1. A green check/tick mark will appear and a button with Copied. This copied url link will be needed to clone the repository to the computer.
   ![clone copied](images/03clonerepo2.png)

1. Install Git (Version Control System) on your computer via this link [Git download](https://git-scm.com/download)

   - Git is needed to store and track any changes made to the downloaded repository, that is on the computer.
   - Git is used to 'push' any changes made to the files in the downloaded repository on the computer back to github.

1. Open a terminal on your computer:

   - Apple Mac: click on Spotlight search and type the word terminal
   - Windows: install Git Bash and open the program
   - Linux: press the keyboard combination Ctrl+Alt+T

1. Navigate to the folder on your computer where you want to copy the github repository. Type `git clone` and paste the repository url; then press enter on the keyboard.
   ![folder clone](images/03clonerepo3.png)
   Open the folder that has just been created, the contents of the repository will be shown.

### Flag Issues

It is vital to share, with the maintainer, that a bug has been found in the project. This helps to improve the project, and makes it easier to use.
To notify the repository owner that a bug has been found in the project, do the following:

- Click on the 'Issues' tab at the top left of the repository.
  ![issues](images/06issues1a.png)

- Has the issue already been raised? Look through the list.
  ![issues](images/06issues2.png)

- If the issue hasn't been raised, then you can inform the repo owner.
- Click on the green 'New issue' button on the right.
  ![new issue](images/06issues3a.png)

- Give the issue a meaningful title and description. And ask if you would like to fix the bug you found.
  ![new issue](images/06issues4.png)

- Your issue will be recorded in the repository. The raised issue will be assigned an issue number.
  ![issue received](images/06issues5.png)

### Make Changes

To make changes to the downloaded repository, it is best to use a Code Editor. Use your favorite editor. Or if you don't have a code editor, here are some examples:

- [VSCode](https://code.visualstudio.com/)
- [Bluefish](https://bluefish.openoffice.nl)
- [Notepad++](https://notpad-plus.org)

1. Using your code editor, open the folder where the repository was copied to.

- Make sure that you are editing the new-branch that was created
- If your code editor supports an integrated terminal, open the terminal within your editor
- In this tutorial, I am using [VSCodium](https://vscodium.com)
- The terminal shows the current working directory (1)

1. **IMPORTANT:** Check which 'branch' is active by typing `git branch` (2)

- current branch is 'main'

- Change to the new-branch name by typing `git checkout "new-branch-name" `

- terminal messages states 'Switched to a new branch "new-branch-name" (3)
  ![branch](images/04newbranch3.png)

- the new branch is also indicated in the bottom corner
  ![branch](images/04newbranch4.png)

1. Make meaningful changes to the file(s) and folders, the source-control icon indicates a change
   ![changes](images/05sourcecontrol.png)

1. **IMPORTANT:** Save the changes made, by using the following commands in the terminal window.
   1. type `git add` command with the name of the file, to stage the changes.
   2. type `git commit -am` command with a message in "quotation marks", to commit the staged changes locally
   3. use the `git push` command to push the changes to the repository stored on GitHub
      ![changes](images/05makechanges3.png)

### Pull Request

A 'pull request' is the way of asking the owner of the original repository that you have made changes to their project.

If the owner agrees that the changes improves the their project, they will 'merge' the changes you have made to their repository.

- go to the origin repository where you 'forked' the project
- click on the green button 'Compare & pull request'
  ![pull request](images/06pullrequest1.png)

A new window will appear to 'Open a pull request'

- write a polite respectful message to the owner of the original repository outlining the changes you have made and how this might improve the project
- click on the green button 'Create pull request'
- wait for the owner of the project to acknowledge the pull request and respond.
  ![create pull request](images/06pullrequest2.png)
