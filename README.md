## Who's a contributor?
If you want to contribute changes to the project and are willing to use the git workflow below, then it can be you.

## Branches defined
* master [Stable]
* dev [Testing]
* If hosted on GitHub: gh-pages


***

## First time using Git?

### Configure Git

### Local Configuration:

**Run the following commands:**

    git config --global user.name "Firstname Lastname"
    git config --global user.email user@example.com
    git config --global color.ui "auto"
    git config --global pack.threads "0"
    git config --global diff.renamelimit "0"
    git config --global core.autocrlf "input"
    git config --global branch.autosetupmerge true

### Github Configuration:

Special settings found on github in the "Account Settings" tab is a point "Global git config information". Please use the two git commands described there:

    git config --global github.user username
    git config --global github.token token

## Ready to start contributing?

### 1. Go to: http://github.com/Code-For-Miami, find the project you are interested in and fork it, then clone your forked repository into the desired directory on your machine.
    cd path/to/desired/directory-name
    git clone git@github.com:YOUR-USERNAME/NAME-OF-THE-FORKED-REPO.git

### 2. To keep your fork up to date you’ll need to create an upstream remote from the Code for Miami project repository:
    cd <directory-name>
    git remote add upstream git://github.com/Code-For-Miami/NAME-OF-REPO-YOU-FORKED.git
    git fetch upstream

### 3. Create a new branch from our dev branch.

We won’t consider any pull requests for commits that are made directly in any of these branches: master or gh-pages.


### Working in the dev branch

### 1. Always make sure you’re on dev branch. You’ll see an asterix by the branch that is checked out.
    git branch

If your branch is not checked out:
    git checkout dev

### 2. Updating your fork from the Code for Miami repo
    git pull upstream package
__NOTE:__ If you have any conflicts, you will need to fix the affected file manually and `git add file-name`

### 3. Change files. Then add and commit.
    git commit -am “My commit message”

### 4. Push changes.
    git push

### 5. Issue a pull request.


***

**If you’re not familiar with Git and GitHub, here are some links we’ve found helpful:**

https://help.github.com/articles/fork-a-repo

https://help.github.com/articles/syncing-a-fork

https://help.github.com/articles/creating-a-pull-request
