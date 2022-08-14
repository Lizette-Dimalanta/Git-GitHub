# __Git & GitHub__

Wednesday, 10 August 2022.

## What is Version Control?
- Also referred to as _source control_ or _revision control_.
- Helps keep track of large groups of files.
- Allows multiple people to work at once without conflict (versions).
- Popular Systems: Git, SVN, Mercurial

## What is Git?
- Open Source Version Control System.
- Runs locally on computer
- Works with repositories, complete history and version tracking.

### Why Do We Need Git?
- Creates a history of changes with full-transparency.
- Allows rollback to previous commit due to possible error (last _'savepoint'_).

## What is GitHub?
- Web-App owned by Microsoft.
- Cloud-based git system repository.
- Shared easily online.

# Terminology
- ### `SSH`: __Secure Shell Protocol__
    - Connects and authenticates to remote servers and services.
    - Git: Can connect to GitHub without supplying username.
        - _Personal access token_ at each visit.

- ### __Repository__
    - A folder where all files are stored.
    - Contains complete history and version-tracking capabilities.

- ### __Working Directory__
    - Root directory on device with source files

- ### __Fork__
    - Create your own remote repo from someone else's with all of the history up to the time of the fork.
    -  Not the same as a branch

- ### __Clone__
    - Copy the contents of a remote repo to your local repo and working directory.

- ### __Master__
    - The default branch on a repository.

- ### __Origin__
    - The default name of the connection to the remote repository.

# Git Flow
![Git Flow](https://res.cloudinary.com/practicaldev/image/fetch/s--M_fHUEqA--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/128hsgntnsu9bww0y8sz.png)

### __Creation__
1. Create file
2. `git init`
3. `code .`

### __Building__
4. `git add .`
5. `git commit -m "Initial Commit/Description"`

### __Uploading__
6. `git remote -v`
7. `git remote add origin "https://https://github.com/Lizette-Dimalanta/Repository"`
8. `git push -u origin master/main`

## Adding Git to GitHub
1. Select _New Repository_ on GitHub.
2. Review settings. Change settings (SSH)
3. Go back to local repository.
4. `git remote -v`: Checks if any local repositories are connected to GitHub.
5. `git remote add origin "link to github"`: Adds repository to GitHub (Only done first time)
6. `git push -u origin master/main`: Connects local repository to remote through SSH key.

# Cheat Sheet

## Useful Resources:
Git Cheat Sheet by GitHub: [Click Here](https://education.github.com/git-cheat-sheet-education.pdf)

Git Cheat Sheet by Atlassian [Click Here](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet)

Git Cheat Sheet by FreeCodeCamp [Click Here](https://www.freecodecamp.org/news/git-cheat-sheet/)

Git Cheat Sheet by GitLab [Click Here](https://about.gitlab.com/images/press/git-cheat-sheet.pdf)

### __Initial Commit__: `git init`

 - Turns any directory into a Git repository.

    __GitHub Source (Init): [Click here](https://github.com/git-guides/git-init)__

### __Clone:__ `git clone https://github.com/github/training-kit.git`

- Creates a copy of specific repository.
- Cloning: Includes all files, branches and commits.

### __Staging Area:__ `git add [file]`

`git add .` : Adds all files in repository

- Moves all selected files onto _staging area_.
- Staging Area: aka. "_to review_".
- Temporary storage for changes in working directory.

    __GitHub Source (Add): [Click here](https://github.com/git-guides/git-add)__

### __Commit:__ `git commit`
1. `git commit -m "Descriptive Commit Message"`

2. `git commit -am "Descriptive Commit Message"`: Add + Commit

- Aka. "_Savepoint_"
- Includes metadata in addition to contents and message: author, timestamp etc.

    __GitHub Source (Commit): [Click here](https://github.com/git-guides/git-commit)__

### __Remote:__ `git remote`
1. `git remote -v`: Lists current remotes associated with local repository.
2. `git remote add [name][origin]`: Add a remote
3. `git remote remove [name]:` Removes a remote
- Manages set of remotes that you are tracking with your local repository.
- Prompts communcation with remote: `git push`, `git clone`, `git pull` and `git fetch`.
   
    __GitHub Source (Remote): [Click here](https://github.com/git-guides/git-remote)__

### __Status:__ `git status`
- Shows current state of your Git working directory and staging area.
    1. Branches
    2. Commits
    3. Staged (or not)

    __GitHub Source (Status): [Click here](https://github.com/git-guides/git-status)__

### __Pull:__ `git pull`
- A combination of `git fetch` + `git merge`.
- Updates current local working branch, all of the remote tracking branches.

    __GitHub Source (Pull): [Click here](https://github.com/git-guides/git-pull)__

### __Push:__ `git push`
`git push -u [remote/origin/branch/master]`
- Aka. _update_ or _publish_
- Uploads all local branch commits to the corresponding remote branch.

    __GitHub Source (Push): [Click here](https://github.com/git-guides/git-push)__

### __Branch__: `git branch --all`
- Keeps track of the branches that you work on locally, as well as each of the branches in every remote associated with your local repo.
- Long list of branches:  
    - Red branches -> Remote tracking branches (read only)

