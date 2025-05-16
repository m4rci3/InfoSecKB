### What is a .git folder?

It stores all the information and metadata about your project’s history, branches , commits, and more. Essentially acting as the brain of your project. it is initialized by `git init` 

This is not all that the *.git* folder has to offer , but if you check the references section below , you can see a more extensive lists and descriptions. 

| Content | Description |
| --- | --- |
| `HEAD` File | Keeping Track of Your Current Branch |
| `refs` Folder | Storing References to Commits and Branches |
| `objects` Folder | Storing Your Codebase as a Series of Snapshots |
| `config` File | Storing Configuration Information for Git |
| `hooks` Folder | Running Scripts at Specific Points in the Git Workflow |
| `logs` Folder | Stores a record of all the changes you made. if you open the file you will find information about the log details |

---
References: 

https://dev.to/rajaniraiyn/understanding-the-contents-of-the-git-folder-ef#:~:text=The%20objects%20folder%20is%20where,two%20subfolders%3A%20pack%20and%20info

https://stackoverflow.com/questions/29217859/what-is-the-git-folder