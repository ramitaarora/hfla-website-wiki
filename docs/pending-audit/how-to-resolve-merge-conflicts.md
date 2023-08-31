# How to use this guide #

Resolving a merge conflict is a complex task that requires you to identify where the problem is coming from before being able to make a decision on which way to resolve it. If this is your first time encountering a merge conflict, I would recommend you read through [What is a merge conflict](#what-is-a-merge-conflict) or do some furthur research to get a better understanding. Otherwise if you already have some understanding of what a merge conflict is, you can follow the steps below to resolve it.

As you go through the steps, please click on the highlighted section links for more in-depth details and example outputs.

### Step 1 : Identify the type of merge failure ###
* Read the very first Git merge error message in your terminal to determine whether it **FAILED TO START** or **FAILED DURING THE MERGE**, using [Types of merge failures](#types-of-merge-failures) as a reference
* If **FAILED TO START** : 
  * The resolution of this error message depends on what you want to do. You can discard your local changes and pull the ones in the repository or you can save your local changes into a stash and pull the version from the repository. It all depends on your preference.
  * There are 4 options provided in detail at this external web page [Fixed: ‘Local changes to following files will be overwritten’ Git Error](https://appuals.com/how-to-fix-git-error-your-local-changes-to-the-following-files-will-be-overwritten-by-merge/)
  * You can also refer to this sub-section [Commands for Merge Fails at the Start ](#commands-for-merge-fails-at-the-start) to decide which commands to use
* If **FAILED DURING THE MERGE** : 
  * We have a hint from Git that there is a merge conflict, continue to Step 2 below to fix confict

### Step 2 : [Identify conflict files](#how-to-identify-which-file-have-conflicts) ### 
* Use `git status` to list out all conflicted files:
  ```bash
  git status
  ```

### Step 3 : [Identify conflict lines in file](#how-to-find-conflicts-within-the-file)
* Use either terminal command or Git command to display the difference in conflicted lines of code:
  * [Using terminal command](#using-terminal-command) :
    ```bash
    $cat <fileName>
    ```
  * [Using Git command](#using-git-command) : 
    ```bash
    git diff
    ```

### Step 4 : [Resolve merge conflict](#how-to-resolve-merge-conflicts)
* If you are using Visual Studio Code as editor, you have the option to use the GUI without manually editing the code. Follow this sub-section to proceed: [Resolving with VSCode](#resolving-with-vscode). Otherwise you still have the option to manually edit the conflict if needed, follow steps below. 
* Manually edit the conflict file by following steps here: [Resolving by editing the file itself](#resolving-by-editing-the-file-itself)

### Step 5 : [What to do after editing](#what-to-do-after-editing) - Adding and commiting your changes
* Once you've reviewed, edited, SAVED your file and resolved your merge conflicts, you can then add your files and commit them as normal:
  * Use `git add <fileName>` to add modified file individually or `git add .` to add all modified files
  * Then `git status` to check if staged correctly
  * Then `git commit -m "Your commit message here"`
  * Then `git status` to check if committed correctly
* After committed the resolved changes, you may resume your `git merge` or `git pull` that you were doing before encounter the merge conflict

### Step Extra: Tools - [Commands for resolving Git merge conflicts](#commands-for-resolving-git-merge-conflicts)

> ***

### External Resources ###
* Github Docs - [Resolving a merge conflict using the command line](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-using-the-command-line)
* Git Documentation - [Reference for Git commands](https://git-scm.com/docs)
* Methods for merge fail to start: [Fixed: ‘Local changes to following files will be overwritten’ Git Error](https://appuals.com/how-to-fix-git-error-your-local-changes-to-the-following-files-will-be-overwritten-by-merge/)
* VS Code Documentation: [Using Git source control in VS Code](https://code.visualstudio.com/docs/sourcecontrol/overview)





***

# **What is a merge conflict?** #

Version control systems like Git are all about managing contributions between multiple distributed authors (usually developers). Sometimes multiple developers may try to edit the same content. If Developer A tries to edit code that Developer B is editing a conflict may occur. To alleviate the occurrence of conflicts developers will work in separate isolated branches. The `git merge` command's primary responsibility is to combine separate branches and resolve any conflicting edits.

> ### Understanding merge conflicts ###
> Conflicts generally arise when two people have changed the same lines in a file, or if one developer deleted a file while another developer was modifying it. In these cases, Git cannot automatically determine what is correct. Conflicts only affect the developer conducting the merge, the rest of the team is unaware of the conflict. Git will mark the file as being conflicted and halt the merging process. It is then the developers' responsibility to resolve the conflict.

[Back to Top](#how-to-use-this-guide)
***

# Types of merge failures #
There are 2 ways in which `git merge` (or a `git pull`, which is a `git fetch` and then a `git merge`) can fail:

* ### Git fails to start the merge ###
  A merge will fail to start when Git sees there are changes in either the working directory or staging area of the current project. Git fails to start the merge because these pending changes could be written over by the commits that are being merged in. When this happens, it is not because of conflicts with other developer's, but conflicts with pending local changes. The local state will need to be stabilized using `git stash`, `git checkout`, `git commit` or `git reset`. You need to modify or stash the files it lists, and then try to do a git pull again. A merge failure on start will output the following error message: 
  ```bash
  error: Entry '<fileName>' not uptodate. Cannot merge. (Changes in working directory)
  ```
  OR
  ```bash
  error: Entry '<fileName>' would be overwritten by merge. Cannot merge. (Changes in staging area)
  ```
  OR
  ```bash
  error: Your local changes to the following files would be overwritten by merge:
        <fileName>
  Please commit your changes or stash them before you merge
  ```
> The 'merge failed to start" error message may be different than what's shown here depending on your Git version, but the message content would be more or less the same: telling you that you have local changes not staged or not commited, and that you need to take care of it or else it would be overwritten by the merge 

* ### Git fails during the merge ###
  A failure DURING a merge indicates a conflict between the current local branch and the branch being merged. This indicates a conflict with another developer's commited changes. Git will do its best to merge the files but will leave things for you to resolve manually in the conflicted files. A mid-merge failure will output the following error message:
  ```bash
  CONFLICT (content): Merge conflict in <fileName>
  Automatic merge failed; fix conflicts and then commit the result.
  ```

[Back to Top](#how-to-use-this-guide)

***
# How to identify which file have conflicts #
> If your merge fail to even start, there will be no merge conflicts in file in the error message as shown in [Types of merge failure: Git fails to start the merge](#types-of-merge-failures). <br>

If Git finds conflicts during the merge, it will list all files that have conflicts after the error message as shown in [Types of merge failure: Git fails during the merge](#types-of-merge-failures). You can also check on which files have merge conflicts by doing a `git status`, which will output as the following:
```bash
$ git status
On branch <current branch>
You have unmerged paths.
(fix conflicts and run "git commit")
(use "git merge --abort" to abort the merge)

Unmerged paths:
(use "git add <file>..." to mark resolution)

both modified:   <fileName>
```

[Back to Top](#how-to-use-this-guide)

***

# How to find conflicts within the file #

* ### Using terminal command ###
  You can examine the conflicted file and see what lines/area in the file that caused the conflicts by using the `cat` command in the terminal:
  ```bash
  $ cat <fileName>
  ```
  then the output would show as the following:
  ```git
  <<<<<< HEAD
  this is where it will show content or lines of code 
  that already exists in the current branch before merge intiated
  =======
  this is where it will show conetent or lines of code
  that you committed in the new branch that you are trying to merge into
  the current branch
  >>>>>>> new-branch-to-merge
  ```

  Think of these new lines as "conflict dividers". The` ======= `line is the "center" divider of the conflict. All the content between the `<<<<<<< HEAD` line and the "center" is content that exists in the current branch which the HEAD ref is pointing to. Alternatively all content between the center and `>>>>>>> new_branch_to_merge` is content that is present in your merging branch.

* ### Using Git command ###
  Alternatively, you can use `git diff` to see the difference between this branch and the one we are merging into:
  ```bash
  git diff
  ```
  Example output:
  ```
  ++<<<<<<< HEAD
   +Some  a
   +Some b
   +Some conflict c 
   +Some conflict d
   +Some e
  ++=======
   + Some conflict 1
   + Some b
   + Some conflict c
   + Some conflict 2
   -Some f
   ++Some f
  ++>>>>>>> main
  ```

[Back to Top](#how-to-use-this-guide)

***

# How to resolve merge conflicts #

* ### Resolving by editing the file itself ###
  The most direct way to resolve a merge conflict is to edit the conflicted file. Open the conflicted file in your favorite editor or IDE and manually edit the conflicted lines. This may mean that you need to make a decision on discarding either your changes or someone else's or doing a mix of the two. You will also need to delete the conflict dividers `<<<<<<<`, `=======`, and `>>>>>>>` in the file.

  * As an example using the output within the previous section [How to find conflicts within the file](#how-to-find-conflicts-within-the-file)
    * If you want to keep ONLY the code change that is already on the current branch, delete all code BELOW the center divider and your file should look like this after edited:
    ```
      this is where it will show content or lines of code 
      that already exists in the current branch before merge intiated
    ```
    * If you want to keep ONLY the new code changes from the merging branch, delete all code ABOVE the center divider and your file should like this after edited:
    ```
      this is where it will show conetent or lines of code
      that you committed in the new branch that you are trying to merge into
      the current branch
    ```
    * If you want to keep BOTH changes, edit to combine both changes and your file should look like this after edited:
    ```
      this is where it will show content or lines of code 
      that already exists in the current branch before merge intiated      
      this is where it will show conetent or lines of code
      that you committed in the new branch that you are trying to merge into
      the current branch
    ```
* ### Resolving with VSCode ###
  > If you need more complex conflict editing guidance with VSCode, checkout the VSCode Documentation on [Using Git source control in VS Code](https://code.visualstudio.com/docs/sourcecontrol/overview)

  If you’re using a modern code editor like Visual Studio Code, then merge conflicts will appear in the GUI where you can accept incoming changes or accept the current changes on your branch. This provides a pretty easy way to fix your conflicts with a few mouse clicks. In Visual Studio Code, this is represented in conflicting files via the GUI shown below. You have a number of options:

  * “Accept Current Changes” - this will use your current branch’s content.
  * “Accept Incoming Changes” - this will use the content from the branch you are merging in.
  * “Accept Both Changes” - this will keep both, one under the other.
  * “Compare Changes” - this will bring up an additional screen to compare changes side by side.

  ![vscode merge conflict GUI example](https://fjolt.com/images/misc/20221023.webp)

[Back to Top](#how-to-use-this-guide)

***

# What to do after editing #
  Once file has been edited, make sure you SAVE the changes on your editor, then use `git status` to check if the conflict messages is still showing ([example conflict message after git status](#how-to-identify-which-file-have-conflicts)); otherwise if the conflict is resolved it should show normal output for `git status`, listing the modified files to be staged:
  ```bash
  On branch <current branch>
  Changes not staged for commit:
    (use "git add <file>..." to update what will be committed)
    (use "git restore <file>..." to discard changes in working directory)
          modified:   <fileName>

  no changes added to commit (use "git add" and/or "git commit -a")
  ```
  After conflict is confirmed resolved, use `git add` to stage the new merged content:
  ```bash
  git add <fileName>
  ```
  > It's best practice to always use `git status` again after `git add` to check if files were staged correctly, same goes for commits before push.

  To finalize the merge, create a new commit by executing:
  ```bash
  git commit -m "merged and resolved the conflict in yourFileName"
  ```

[Back to Top](#how-to-use-this-guide)

***

# Commands for resolving Git merge conflicts #
### General Commands ###
Git status is the most frequently used command to display the status of modified files, staging area, and commits. During the merging process, it is used to identify conflicted files.  
```
git status
```

The Git log with --merge arguments produces the list of commits that are in conflict with the source branch. 
```
git log --merge
```

By default, the `git diff` option will show you the difference between uncommitted changes and previous commits. Git diff is used for comparing branches, commits, and files. It is useful for preventing future merge conflicts. 
```
git diff
```
### Commands for Merge Fails at the Start ###
>  IMPORTANT: Do not use git stash if git went through with the merge and there were merge conflicts! Only use git stash if git refused to merge because it foresees there being conflicts.

The `git stash` command stashes away any changes in your staging area and working direcotry. It's useful in saving all changes not ready to be committed and the user wants to have an updated repository

Save changes to file in working directory and staging area that Git is aware of
```
$ git stash save "Your save message"
```
Removes the most recent stash or any stash specified and applies changes as a merge. If merge fails the stash is not removed from the list and must be removed manually.
```
git stash pop
```
The checkout is used for undoing changes or switching to a new or old branch. 
```
git checkout
```
The Git reset is for reverting the changes in the working directory and staging area. 
```
git reset --mixed
```
### Commands for Conflicts During the Merge ###
The --abort argument will stop the merge process and revert the changes to their original state before the merge started. 
```
git merge --abort
```
Git reset is usually used during the merging process to revert the conflicted files to their original state.
```
git reset
```
### Resolve Deleted-Modified File Conflicts ###
Git conflict will occur if you have deleted the file in the current branch, and someone else has modified it in another branch. In this case, you can either add a file and commit,
```
git add <filename>
```
or you can remove the file and commit. 
```
git rm <filename>
```

[Back to Top](#how-to-use-this-guide)