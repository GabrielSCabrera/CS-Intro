# Computational Science Toolkit

A short list and description of tools that are important, convenient, and nice.

1. Git
2. Pipenv
3. Black



## Git
Installation instructions can be found
[here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).


### Basics
Git tracks changes in your repository by keeping track of small "deltas".
Works best with text files.
Git tries to make a linear history.


Create repository:
```bash
git init
```



Add files for tracking:
```bash
git add <files>
```
Pro-mode, use the `--patch`-flag.



Record changes:
```bash
git commit
```
Check [this](https://chris.beams.io/posts/git-commit/) blog post for tips on
writing commit messages.

![](https://imgs.xkcd.com/comics/git_commit.png)



Show status:
```bash
git status
```
Go crazy!



Show history:
```bash
git log
```
Who gets the blame?



Branch out:
```bash
git checkout -b <branch-name>
```
I've just gotta make these changes...



Merge branches into master:
```bash
git merge <branch-name> master
```
__MERGE CONFLICT!!!!__ 😱




### Keep you repository clean!
Only track necessary changes! Use `.gitignore`!



### Hosting
- Github, Bitbucket, GitLab.
- "Social network"
- Attractive and active repos are targets for recruiters! 🎉



### Collaboration
- Collaborators
- Forks
- Pull requests
- Issues



## Pipenv
Keep your Python environments separated!


### Installation

```bash
pip install pipenv
```


### Basics

```bash
pipenv install <package-name>
```
Creates a `Pipfile` and a `Pipfile.lock`.
Keep both the `Pipfile` and `Pipfile.lock` under version control.
Only include `Pipfile` in case of a library.


Activate environment:
```bash
pipenv shell
```
Run normal commands once inside the shell.


Leave environment:
```bash
exit
```


## Black

Yes.

### Installation

```bash
pip install black
```

Or, in the `Pipfile` with:
```bash
pipenv install black==19.3b0
```

### Basics
All there is to it:
```bash
black .
```
