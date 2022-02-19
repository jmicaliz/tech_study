# Git Notes

## Setting up Bare Git Repo
#git #repo #init

```bash
$ cd /srv/git
$ mkdir project.git
$ cd project.git
$ git init --bare
```

## Setting up another server as git remote
#git #remote

```bash
# on local dev box
$ cd myproject
$ git init
$ git add .
$ git commit -m 'initial commit'
$ git remote add origin git@gitserver:/srv/git/project.git
$ git push origin master
```
