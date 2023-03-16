# THIS REPO WAS BORN TO FAIL

# Demo Merge Conflicts Repository

This repository is created to demonstrate and help users understand merge conflicts in Git and GitHub. The primary goal of this demo is to provide a hands-on experience in resolving merge conflicts that arise while collaborating on a project.

## Table of Contents

1. [Introduction](#introduction)
2. [Getting Started](#getting-started)
3. [Simulating Merge Conflicts](#simulating-merge-conflicts)
4. [Resolving Merge Conflicts](#resolving-merge-conflicts)
5. [Additional Resources](#additional-resources)

## Introduction

Merge conflicts occur when two or more developers modify the same lines of code in the same file, or when one developer deletes a file while another developer makes changes to the same file. Git is unable to automatically determine which changes should be kept, so the developers must manually resolve the conflict.

## Getting Started

Before proceeding, make sure you have the following tools installed:

1. Git
2. A text editor (e.g., Visual Studio Code, Atom, Sublime Text, etc.)

To get started, follow these steps:

1. Fork this repository to your own GitHub account by clicking the "Fork" button at the top right of this page.
2. Clone your forked repository to your local machine:
```
git clone https://github.com/YOUR_USERNAME/demo-merge-conflicts.git
cd demo-merge-conflicts
```


## Simulating Merge Conflicts

To simulate a merge conflict, follow these steps:

1. Create a new branch:
```
git checkout -b your-feature-branch
```
2. Open the `sample.txt` file in your preferred text editor and make some changes.
3. Commit the changes:
```
git add sample.txt
git commit -m "Made changes in your-feature-branch"
```
4. Switch back to the `main` branch:
```
git checkout main
```
5. Make changes to the same lines in the `sample.txt` file as in step 2.
6. Commit the changes:
```
git add sample.txt
git commit -m "Made changes in main branch"
```
7. Merge your `your-feature-branch` into the `main` branch:
```
git merge your-feature-branch
```

You should now see a message indicating that there is a merge conflict.

## Resolving Merge Conflicts

To resolve the merge conflict, follow these steps:

1. Open the `sample.txt` file in your text editor.
2. Look for the conflict markers (`<<<<<<<`, `=======`, and `>>>>>>>`), and edit the file to keep the desired changes.
3. Remove the conflict markers.
4. Save and close the file.
5. Stage and commit the resolved file:

```
git add sample.txt
git commit -m "Resolved merge conflict"
```
6. Push the changes to your remote repository:
```
git push origin main
```

The merge conflict should now be resolved.

## Additional Resources

For more information about Git and handling merge conflicts, consider the following resources:

1. [Pro Git Book](https://git-scm.com/book/en/v2)
2. [GitHub Help: Resolving a merge conflict](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/resolving-a-merge-conflict-using-the-command-line)

Feel free to contribute to this repository by submitting a pull request or opening an issue if you have any suggestions or improvements. Happy coding!
