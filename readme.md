# Uploading Files To Github  Locally with Git Bash

- You need a github account
- Download git bash here (https://git-scm.com/downloads)

## Creating an empty repository on github
- Create or connect to github accout
- Under your profile in the upper right, find `your repositories`
- Click `new`
- Create a repository name
- Click `create repository`
- Click on your newly created repository
- Copy the path beginning with `https://github.com/username/test.git`
- Paste it in a simple text file, we will use it later.*

## Uploading source code with git

1- Hold `Windows` and `s` type `bash`

2- Change directory to the folder you want to upload running `cd`

3- Run `git init` . 

Output will be something similar to this:
`Initialized empty Git repository in C:/Users/username/Desktop/yourfolder/.git/`

4- Run `git remote add origin [paste the path you copied before]`

5- you will check whether you have fetch and push acccess by running `git remote -v`


6- Run `git add .` to upload all the files in the current directory

7- Run `git commit -m "First Commit"`

8- Run `git push origin master`

Then you can refresh the path to verify the update.

* I got **`Git fatal: protocol 'https' is not supported` error** because of directly pasting the path. Although invisible in bash, there were clearly unrecognized charaters preceeding the https link when I pasted ot to a simple editor. 

## Summary
#### Helpful Commands

```
git help
git init
git remote add origin [paste the path of your newly created repo]
git remote -v
git add .
git commit -m "First commit"
git push origin master




