# GIT

Git is a fast, scalable, distributed revision control system with an unusually rich command set that provides both high-level operations and full access to internals.
#### OPTIONS

**-v,--version** 

   Prints the Git suite version that the git program came from.

    git -v, git --version


**-h,--help** 

  Prints the synopsis and a list of the most commonly used commands.

    git -h, git --help

## Commands
    
### CLONE

**git-clone** - Clone a repository into a new directory Clones a repository into a newly created directory, creates remote-tracking branches for each branch in the cloned repository

    git clone git@github.com:eugenewere/Documentation.git

Cloning specific branch by using **-b [branch-name]**

    git clone -b [branch-name] git@github.com:eugenewere/Documentation.git

### INIT

 **git init** - Create an empty Git repository or reinitialize an existing one

    git init 

 **-b [branch-name]**

 Use the specified name for the initial branch in the newly created repository. If not specified, fall back to the default name (currently master, but this is subject to change in the future

    git init -b master

### ADD 

**git add ./[filename]** - This command updates the index using the current content found in the working tree, to prepare the content staged for the next commit. It typically adds the current content of existing paths as a whole, but with some options it can also be used to add content with only part of the changes made to the working tree files applied, or remove paths that do not exist in the working tree anymore.

    git add .  #all files
    git add [filename] # specific files

 **git add -f/--force** - Allow adding otherwise ignored files by force.

    git add --force (. or [filename])
    git add -f (. or [filename])


### STATUS 

**git status** - Displays paths that have differences between the index file and the current HEAD commit, paths that have differences between the working tree and the index file, and paths in the working tree that are not tracked by Git

**-s, --short**

Give the output in the short-format.

    git status -s

**-b, --branch**

Show the branch and tracking info even in short-format.
    
    git status -b master

### COMMIT

**git commit** - Create a new commit containing the current contents of the index and the given log message describing the changes. The new commit is a direct child of HEAD, usually the tip of the current branch, and the branch is updated to point to it

**-m [msg] --message=[msg]**
Use the given <msg> as the commit message. If multiple -m options are given, their values are concatenated as separate paragraphs.

    git commit -m "initial commit"

**--amend**

Replace the tip of the current branch by creating a new commit

     git commit --amend

### RESET

**git-reset** - Reset current HEAD to the specified state

**git reset [mode] [commit]**
This form resets the current branch head to <commit> and possibly updates the index (resetting it to the tree of <commit>) and the working tree depending on <mode>. Before the operation, ORIG_HEAD is set to the tip of the current branch. 

- **--soft**

    Does not touch the index file or the working tree at all (but resets the head to <commit>, just like all modes do). This leaves all your changed files "Changes to be committed", as git status would put it.

- **--mixed**

    Resets the index but not the working tree (i.e., the changed files are preserved but not marked for commit) and reports what has not been updated. This is the default action.


- **--hard**

    Resets the index and working tree. Any changes to tracked files in the working tree since <commit> are discarded. Any untracked files or directories in the way of writing any tracked files are simply deleted.



