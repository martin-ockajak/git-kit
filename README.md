# Overview

**Git Kit** is a simple tool for enhancing the usability of Git by providing several convenient aliases.

The functionality is similar to and can be considered an extension of [Git Extras](https://github.com/tj/git-extras).

* [Aliases](#aliases)
* [Examples](#examples)
* [Installation](#installation)


# Aliases

* **fuse** - Pull changes from all remote branches and push changes to the current branch.
* **amend** - Add staged changes to the last commit.
* **pullmerge** - Merge a branch into the current branch using the last revision of both branches.
* **blankmerge** - Merge a branch into the current branch without applying any changes.
* **graphlog** - Display commit log for all branches as a graph.
* **branchlog** - Display commit log for specified branch only.
* **kit** - List Git aliases invoking Git Kit commands.


# Installation

**Requirements**

* [Git](https://git-scm.com/)
* [Python](https://www.python.org/)
* [cURL](https://curl.se/) (for quick installation only)

Run the following command from within root directory of a Git repository to install *Git Kit* into it:
```bash
curl https://raw.githubusercontent.com/martin-ockajak/git-kit/main/git-kit | python3 - install .
```

Alternatively, *Git Kit* can also be downloaded used directly as a script without installation.


# Examples

**Display Git command aliases invoking Git Kit commands.**
```
git kit
```

**Display help for specified Git Kit operation.**
```
git <operation> -h
```

**Synchronize changes to checked out branches.**
```
git fuse
```

**Synchronize changes to all branches.**
```
git fuse -a
```

**Synchronize changes to checked out branches and delete local branches tracking non-existent remote branches.**
```
git fuse -p
```

# Inspired by

* [Gitless](https://gitless.com/)
* [Mercurial](https://www.mercurial-scm.org)

