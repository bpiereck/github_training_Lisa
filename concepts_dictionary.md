# Dictionary

1. Git: Specific to a project, contains a timeline within that project. Version control system in which one can control changes and reverte to previous states.

2. GitHub: collection of different gits. Is a cloud-based system that collects different Gits.

3. Conceptual areas: 
- Developing area: is the project folder that was initiated as a git repository

- Local repository: hidden file .git where all the changes are being tracked and kept (timeline)

- Staging area: location used to prepare new snapshots to the timeline. Temporary, intermediary area to prepare the commit. This area is important because it allows you to organize your files. You can add several files for which changes are linked and then commit both files together with only one message.

>What happen if I forget the `-m` in my commit?
It opens a text editor and allows you to write a longer message (unlimited characters)

4. Files to ignore in GitHub
create a file called `.gitignore`, list files and folders that will not be version-controlled by Git, nor pushed to GitHub

5. README.md file
Is the file to describe your project, tool in Git and GitHub. Very important and very good practice in RDM.git add

6. How to go from your local to your remote
You create "a bridge" or connection, while to send commit through the bridge you need 

7. How to collaborate?
You invite the collaborators through github.com. You go to the repository on github, click settings, collaborators in the left panel, click the green 'Add people' button and add their username or email adress.
When someone has invited you, after accepting, you clone the repository locally (not in a folder already tracked by git) and can start making changes. To save the changes you do the normal git add, git commit -m 'message' and git push.

8. Git branch: You can create a branch to work on your code without affecting the original code tht is in the main branch.

Mirror effect: you will see in your folder, all the copies of the files that are in the branch where you are.

9. Detached head:

You detach a version of your code to a separated head that will not be linked to the main or another branch. It is possible to immediately link it back to a branch or later (but more complex).

10. Tagging: it enables you to mark a specific release or version of your code. The tags will also enable you to download a .zip file of your remote repository once on GitHub.

Bruna Piereck
