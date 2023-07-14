# Overview

**GitMore** is a simple tool for enhancing the usability of Git by providing several convenient aliases.

* [Aliases](#aliases)
* [Examples](#examples)
* [Installation](#installation)


# Aliases

* **sync** - Pull changes from all remote branches and push changes to the current branch.
* **amend** - Add staged changes to the last commit.
* **pullmerge** - Merge a branch into the current branch using the last revision of both branches.
* **blankmerge** - Merge a branch into the current branch without applying any changes.
* **graphlog** - Display commit log for all branches as a graph.
* **branchlog** - Display commit log for specified branch only.
* **createbranch** - Create a local branch and push its tracked remote branch.
* **deletebranch** - Delete both a local branch and its tracked remote branch.
* **more** - List Git command aliases invoking GitMore operations.


# Installation

**Requirements**

* [Git](https://git-scm.com/)
* [Python 3](https://www.python.org/)
* [cURL](https://curl.se/) (for quick installation only)

Run the following command from within root directory of a Git repository to install *GitMore* into it:
```bash
curl https://raw.githubusercontent.com/martin-ockajak/gitmore/main/gitmore | python3 - install .
```

Alternatively, *GitMore* can also be downloaded used directly as a script without installation.


# Examples

**Display Git command aliases invoking GitMore operations.**
```
git more
```

**Display help for specified GitMore operation.**
```
git <operation> -h
```

**Synchronize changes to checked out branches.**
```
git sync
```

**Synchronize changes to all branches.**
```
git sync -a
```

**Synchronize changes to checked out branches and delete local branches tracking non-existent remote branches.**
```
git sync -p
```

# Inspired by

* [Gitless](https://gitless.com/)
* [Mercurial](https://www.mercurial-scm.org)

