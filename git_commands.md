# Git and Github

Here is a list of quick commands to do most typical tasks

## Creating repo from local files and pushing GitHub

FIRST create the repo on github e.g - https://github.com/dalyw01/my_new_repo

```
git init
git add .
git commit -m "first commit"
git remote add origin https://github.com/dalyw01/my_new_repo.git
git push -u origin master
```

## Downloading online repo code, setting up new branch from and commiting to the NEW branch

FIRST have the link to the repo you want to clone handy e.g - https://github.com/dalyw01/my_new_repo

```
mkdir x
cd x
git init
git clone https://github.com/dalyw01/smp-ui-tests
git remote add origin https://github.com/dalyw01/smp-ui-tests.git
git add .
git commit -m "asdadads"
git branch wills_branch 
git checkout wills_branch    
git push -u origin wills_branch
```
## Downloading specific branch of a repo

Make a folder and enter it

```
mkdir apple
cd apple
```

Download the branch "NihalBranch" from project "Test-Combos-For-Web" owned by dalyw01 into apple

```
git clone -b NihalBranch git@github.com:dalyw01/Test-Combos-For-Web.git
```

Jump into the folder

```
cd Test-Combos-For-Web/
```

Verify on different branch

```
git branch
* NihalBranch
```

## Setting a new remote after breaking previous

```
git remote set-url origin https://github.com/dalyw01/Scanner.git
git pull origin master
```