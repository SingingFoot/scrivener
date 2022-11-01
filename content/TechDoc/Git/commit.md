+++
title = "How to make commits locally and globally"
description = "This is an area for technical documentation"
weight = 1
+++

1. After you created new repository with {git init} or cloned an existing repository with {git clone {repository address}}, open your terminal in the local repository folder with the command:

    ```
    cd {name of repository folder}
    ```

2. After you made some changes in your local repository folder you need to index them with {git add} command: 
    ```
    git add .   ->   add the {space + dot} after {add} to index all the changed files. 
    ```
3. Commit all the changes locally with {git commit} command and a comment.
    ```
    git commit -m 'Add new benchmarks' -> add {-m} mark and a comment in quotation marks. 
    git commit -a -m 'Add new benchmarks' -> add {-a} mark to index all the non-indexed changes you've made.
    ```
4. To make changes globally in your remote repository, use command {git push origin master} or just {git push}:
    ```
    git push origin master
    ```