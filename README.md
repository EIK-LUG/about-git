# about-git-and-github

### A general overview

![git-overview](../images/git-overview.png)

### Terminology

##### Github 

* **Forking** - Creating a copy remote repository. You will have the whole code and can make any changes you please, changes will not affect the original remote repository. 
    * How to fork - On the repositories github page there is a Fork button.
* **Creating a pull request** - This allows you to offer the changes made in your fork back to the original repository. These may or may not be accepted (merged) into the original by the repository administrators.
    * How to create a pull request - A button on your fork repositories github page

##### git

Note: You need to have git installed

* **Cloning** - This will create a local repository copy of the remote repository, which can be edited and then the changes pushed to the remote repository.
    * How to clone - "git clone https_clone_url" https_clone_url can be gotten from the repositories GitHub page.
* **Adding** - This will add a file/folder to be tracked by git. If you just add a new file into your local repository, then it will NOT be tacked by git, until you add it.
    * How to add - "git add file_or_folder_name" or often "git add -a" which will add all files to be tracked
* **Committing** - This will stage a changed or new file/folder for pushing back to the remote repository.
    * How to commit - "git commit file_or_folder_name" or often "git commit -a" which will commit all changes
* **Push** - This will attempt to push all files and folders that are staged for pushing to the remote repository. It might fail if there are changes in the remote repository that are not in your local repository, then just "git pull".
    * How to Push - "git push -u origin master"
* **Pull** - This will pull any changes in the remote repository that are not in your local repository into your local repository.
    * How to pull - "git pull"
    
### What for? (basic version)

NOTE: 99.8% on serious projects are on some version control system. Learn it, your potential employer will not shun you and your colleagues/teammates will thank you.

##### You will have a history of changes.

* There will be a commit history, that will contain all the commits made and the exact lines of codes changed etc. will be shown.
* This also means you can retrieve old code from the history
* This also means you can revert changes in your local repository - pretty much you can screw up as much as you want.

##### Multiple people can easily collaborate on a single code base

* Everyone can see the state of the code base, without asking the others for a copy
* You will have a good way to handle conflicts
* You can make it easy for other people to contribute to your project
* You can monitor work being done on a code base
* You will be able to review changes before merging them into your code

![git-multi-users](../images/git_multi.png)

And much more!

##### On IDE integration 
  
Most good IDEs will have some form of integration with VCSs. However the exact same principles apply for both using the command line and using an IDE for version control.

JetBrain's IDEs (IntelliJ, PyCharm, WebStorm, PhpStorm etc.) all have this feature and usage is easy, just right click and go to "git" in the drop down menu.