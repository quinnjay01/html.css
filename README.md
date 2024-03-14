This is my first read me file

Instructions on how to git for my fies to repository

Terminal command to access my folder html.css.lesson

Directory: C:\Users\quin\UP_RIGHT_PROJECTS\1-html-css\html.css.lesson

PS C:\Users\quin\UP_RIGHT_PROJECTS\1-html-css> cd html.css.lesson
PS C:\Users\quin\UP_RIGHT_PROJECTS\1-html-css\html.css.lesson> ls


Directory: C:\Users\quin\UP_RIGHT_PROJECTS\1-html-css\html.css.lesson


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----         3/13/2024   8:02 PM            527 index.html
-a----         3/13/2024   8:01 PM            234 style.css


PS C:\Users\quin\UP_RIGHT_PROJECTS\1-html-css\html.css.lesson>





GitHub
https://github.com/quinnjay01/html.css.git

Create a new repository on the command line
Step 1: Configure Git with Your Identity
First, set your Git username and email. These are important because every Git commit uses this information, and it's immutably logged in the commits you start creating:
git config --global user.name "quinnjay01"
git config --global user.email "parina61@gmail.com"
Step 2: Initialize a Git Repository
Navigate to your project directory and initialize a Git repository if one doesn't already exist:
cd C:\Users\quin\UP_RIGHT_PROJECTS\1-html-css\html.css.lesson
git init
Step 3: Stage and Commit Your Changes
After adding or modifying files, stage them for commit:
git add .
Then commit your changes:
git commit -m "I am pushing my html and css files"
If you encounter a message saying there's nothing to commit, ensure you've made changes to the files.

Step 4: Connect Your Local Repository to a GitHub Repository
If you've already set a remote called origin, and you need to change its URL:
git remote set-url origin https://github.com/quinnjay01/html.css.git
…………………………………………………………..
If you haven't set a remote or need to add it for the first time:
git remote add origin https://github.com/quinnjay01/html.css.git

Step 5: Push Your Changes to GitHub
Finally, push your changes to GitHub. If you're using the master branch (or main, depending on your Git version or preference), use:
git push -u origin master
This command pushes your commits to the master branch of the remote repository specified by origin and sets the upstream (tracking) reference. For subsequent pushes, you can simply use git push.

Troubleshooting Common Issues
Fatal: protocol 'https' is not supported: This error usually indicates a problem with the remote repository URL. The steps you've followed by setting the correct URL with git remote set-url should resolve this issue.
Error: remote origin already exists: This means you're trying to add a new remote called origin when one already exists. Use git remote set-url to change the existing remote's URL or git remote remove origin followed by git remote add origin to replace it.
Nothing to commit, working tree clean: This message appears if there are no changes detected in your working directory since your last commit. Make sure you've made changes to your files and added them with git add ..
