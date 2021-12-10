# Git
***
## Table of Contents
  - [Table of Contents](#table-of-contents)
  - [version](#version)
  - [config](#config)
  - [states](#states)
  - [init](#init)
  - [remote](#remote)
  - [branches](#branches)
  - [merge](#merge)
  - [update remote repository](#update-remote-repository)
  - [tags](#tags)

## version
> `git --version`

## config
> `git config -l`
>
> `git config --global user.name "Username"`
>
> `git config --global user.email "email@domain.com"`
>
> `git config --system core.editor "/bin/vim"`
>
> `git config --global init.defaultBranch main`


## states
1.  Working directory
    - > `git add <FILENAME_OR_DIRECTORY>`
2.  Staging area
    - > `git commit -m "message"`
3.  '.git' directory (repository)
    - > `git push origin <BRANCH>`  

## init
> `git init <PATH>`


## remote
1.  Display remote repositories
    - > `git remote -v`
2.  Add remote repository
    - > `git remote add origin  <REMOTE_URL>`


## branches 
1.  Display branches
    -  > `git branch -a`
2.  Create branch
    -  > `git checkout -b <BRANCH>`
3.  Change branch
    -  > `git checkout <BRANCH>`
4.  Delete branch
    -  > `git branch -d <BRANCH>`
5.  Delete branch (force)
    -  > `git branch -D <BRANCH>`

## merge
> `git merge <BRANCH>`

## update remote repository
1. Download objects and refs from remote repository
   - > `git fetch`
2. Integrate with another repository or a local branch
   - > `git pull origin <BRANCH>`

## tags

* Listing the existing tags
  * > `git tag`
* Search tags by pattern 
  * > `git tag -l "PATTERN"`
* Create tag
  * > `git tag -a v1.0 -m "tagging message"`
* See tag data
  * > `git tag show v1.0`
* Delete tag
  * > `git tag -d v1.0`
* Push tag
  *  > `git push origin v1.0`