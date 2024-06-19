---
sidebar_position: 2
---

# Commands

There are lot of things you can do with git, but only handfull of commands that we use in our daily basis, Those commands are mentioned below.

1.  ### Initialize a Repository:

    ```bash
    git init
    ```

2.  ### Clone a Repository:

    ```bash
    git clone <repository-url>
    ```

3.  ### Check Status:

    ```bash
    git status
    ```

4.  ### Stage Changes:
    ```bash
    git add <file(s)>
    ```
5.  ### Commit Changes:
    ```bash
    git commit -m "Commit message"
    ```
6.  ### Push Changes:
    ```bash
    git push origin <branch>
    ```
7.  ### Pull Changes:
    ```bash
    git pull origin <branch>
    ```
8.  ### Create a Branch:

        ```bash
        git checkout -b <branch-name>
        ```

9.  ### Switch Branches:
    ```bash
    git checkout <branch-name>
    ```
10. ### Merge Branches:
    ```bash
    git merge <branch>
    ```
11. ### View Commit History:
    ```bash
    git log
    ```
12. ### Undo Changes:

    ```bash
    git reset --hard HEAD~1   # Undo last commit and reset changes
    git checkout -<file>    # Discard changes in a specific file

    ```

13. ### View Differences:

    ```bash
    git diff          # Show unstaged changes
    git diff --cached # Show staged changes
    ```

14. ### Tag a Commit:
    ```bash
    git tag <tag-name>
    ```
15. ### Fetch Tags:

    ```bash
    git fetch --tags
    ```
