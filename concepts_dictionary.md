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