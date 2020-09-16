## Git Flow

The GitFlow Workflow is a model developed for Git by Vincent Driessen, it helps with collaboration amongst the development teams. It allows parallel development of features without disrupting the main branch (master). How it works is as described in the following image

![Image of GitFlow](https://datasift.github.io/gitflow/GitFlowHotfixBranch.png)

1. First  we create and checkout a new branch from the master branch. (shown in light blue on the right).
2. Now we Develop from that branch we just checked out (illustrated by the yellow line) Bugfixes and any feature developments are pushed back here to this branch
3. Then we have the Feature branch which is used to work on certain features of the project one by one (illustrated in pink). A single person or multiple people in a team can work together on this branch and test things without affecting the work of others. When the time comes they can merge these features back to the develop branch
4. Now the Release branch (illustrated in green) is made to test all the changes made in the develop branch to make sure everything works as it is supposed to, and if any fixes need to be made they can do so here.
5. After the release branch is merged in the master branch maybe before release if there are any emergency fixes they will be fixed in the HotFix branch (illustrated in red) once resolved they are merged back into master branch and develop branch.

### Use Case of Git Flow
When we are using git flow, we create a repository firstly, add collaborators and start the project. Basically, we have a remote repository and several local repositories which are cloned from the remote repository or another remote repository which is forked from the original one. We use git add and git commit commands to submit the change in the codes and documents. 
Here is a typical example: Then we add and commit the changes to the local git. After that, we can push them to the remote repository. We can also push them to the forked repository, and then raise a pull request to the original repository. If the repository has been updated by others, we could also pull the changes to the local repository easily.
We can check the status of the git by using git status, which shows us the workspace of the git. We can also use git rm to  remove files from the remote repository and remove commands to remove branches. We can get information on the commits by using git show.

* [Video](https://www.youtube.com/watch?v=47E-jcuQz5c&index=1&list=PLg7s6cbtAD17Gw5u8644bgKhgRLiJXdX4)