# gitlite
This program is a version control system that is similar, but also smaller and simpler than [Git](https://git-scm.com/). A version control system helps a user by saving snapshots of files at times specified by the user,  called commits. This is useful because a user can revert back to old versions in the case of wrong turns or accidently deleted files.

In order to run the program, please first inialise a Gitlite by typing `java Gitlite init` to initalise a gitlite repository. If you're unfamiliar with Git or what this means, it will create a hidden folder that will save the copies of your file(s). "Hidden" means that you will be unable to view the folder in Finder (or Explorer on Windows) or if you type `ls` in the terminal. This is important because it prevents you from accidently deleting your commited files.

Prior to commiting a file, you will have to stage by typing `java Gitlite add [file name]`. In case you accidently change a file or add it unintentially, you can remove it from the staging area by typing `java Gitlite remove [file name]`.

Committing means you are storing a copy of your files at that moment. This creates the various versions you could have of a program, hence the version control system that is Gitlite. To commit, please try `java Gitlite commit [message]`. It's best to make the message something that is applicable to the changes you have made. You may later access the commits by their commit messages.

Your may access a log of your commits by typing `java Gitlite log`. This will tell you the commit number, time and date of the commit, and the commit message you applied to it. This will only give you the history of this node's commit history. In order to view the full history, please type `java Gitlite global-log`.

To find the commit id of a commit, type `java Gitlite find [commit message]`. This will be helpful if you recall what changes you'd like and would also like to know where in your progression it was committed.

---

The design of the project goes through the initial and progressive changes of the architecture of the program. Each design iteration is given a new file because of the large amount of moving parts. For further details about what has changed from iteration to iteration, please click on the commit message to see the greater details of the individual change. Though it may be difficult to understand why

The code of the project does not follow the same new file(s) iteration as the design. The commit log can be viewed as normal.
