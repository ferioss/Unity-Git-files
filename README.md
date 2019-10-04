
## Git Support for Unity Game Engine
Unity engine and some IDEs used by Unity developers create a bunch of temporary files in your project, which you don't want to keep in your repository.

Also while developing games in general, you will have some binary files and assets in your projects, which you need to keep in your repository; but Git is not particularly good at handling large binary files on its own.

These problems can be solved by using a proper `.gitignore` file, and using Git LFS (Large File Support) extension with the proper `.gitattributes` file, both of which are provided in this project.

This repository is a template, which you can use to create new repositories from, and start developing your Unity games!

## What is Git LFS?
Git LFS is an open source extension for Git, which improves Git's behavior regarding large binary files. It replaces large files such as audio samples, videos, datasets, and graphics with text pointers inside Git, while storing the file contents on a remote server like GitHub, GitLab, or BitBucket. This is extremely handy for game development, since your local repository size will remain significantly smaller, and Git operations will be much faster.

## How to use?
Just create a new repository from this one. Alternatively, copy `.gitignore` and `.gitattributes` files and put them in the root of your Unity project. Your project folder should look like this:
![Project root](https://i.imgur.com/maqAXE2.png)

In order to use Git LFS, you will need to install it first. Download the latest client from [git-lfs.github.com](https://git-lfs.github.com) and install it. Once downloaded and installed, set up Git LFS and its respective hooks by running:
`git lfs install`

You are all set!

## Contribute
If your project needs new file types covered in either of the `.gitattribues` or `.gitignore` files, chances are other people will need them too. By creating a pull request with your modified file(s), you will help them out.
