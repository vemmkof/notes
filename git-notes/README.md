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
    * > `git add <FILENAME_OR_DIRECTORY>`
2.  Staging area
    * > `git commit -m "message"`
3.  '.git' directory (repository)
    * > `git push origin <BRANCH>`  
* In each state you can use the following commands to see:
  - Working tree status
    * > `git status`
    * > `git status <PATH>`
  - Commit logs
    * > `git log`


## init
> `git init <PATH>`


## remote
*  Display remote repositories
    * > `git remote -v`
*  Add remote repository
    * > `git remote add origin  <REMOTE_URL>`


## branches 
*  Display branches
    -  > `git branch -a`
*  Create branch
    -  > `git checkout -b <BRANCH>`
*  Change branch
    -  > `git checkout <BRANCH>`
*  Delete branch
    -  > `git branch -d <BRANCH>`
*  Delete branch (force)
    -  > `git branch -D <BRANCH>`

## merge
> `git merge <BRANCH>`

## update remote repository
* Download objects and refs from remote repository
   * > `git fetch`
* Integrate with another repository or a local branch
   * > `git pull origin <BRANCH>`

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

## logging
* One line
  * > `git log --oneline`
* Changes listed
  * > `git log -p`
* Specific file
  * > `git log -- <PATH_TO_FILE>`
* Specific author
  * > `git log --author="<USERNAME>"`
* Specific keyword in commit message
  * > `git log --grep="<KEYWORD>"`
* Specific keyword in commit message (ignore case)
  * > `git log -i --grep="<KeYwOrD>"`
* Graphic log
  * > `git log --graph`

## cloning repos
* local
  * > `git clone <PATH>`
* remote
  * > `git clone <REMOTE_URL>`
* dadas
  * > `git log --graph`


## ignoring
* Configure global file 
  * `git config --global core.excludefile '<PATH_TO_FILE>'`
    * > `git config --global core.excludefile '/etc/gitignore'`

* Local file
  * > `touch .gitignore`

