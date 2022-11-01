+++
title = "How to create a pull request with git"
description = "This is an area for technical documentation"
weight = 2
+++

1. Find a repository where the owner made you a collaborator. You should get a letter with invitation to your mail.
2. Create a fork of the original repository.
3. Create a clone of this forked repository. For that:
a) copy the address of that forked repository;
b) open the folder where you are going to clone this repository;
c) open the terminal inside this folder;
d) write the command: git clone {the address of the forked repository}, for example:
git clone https://github.com/SingingFoot/test
4. Create a new branch "test_branch" inside your cloned folder with command:
git checkout -b test_branch
5. Add some new files or change the existing files into your cloned folder.
6. Push these changes locally:
git add .
git commit -m "new changes"
git push -u origin test_branch
7. Go to the your repository on git and find the button "Compare & pull request".
8. Add some comments and press the button "Create pull request".