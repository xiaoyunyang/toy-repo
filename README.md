# Toy Repo

## Get Good with Git

* [Useful git commands](https://xiaoyunyang.github.io/post/everything-you-need-to-know-about-git/)
* [Backlog Branching Tutorial](https://backlog.com/git-tutorial/branching/switch-branch/)

Practice working with branches

Create new repo called toy-repo, then clone local:

```
$ cd toy-repo
```

Add README to master

```
$ touch README.md
$ git commit -m 'added README'
$ git add .
$ git push origin master
```

Create branch1 and branch2 such that branch1 has README.md and branch1.md while branch2 has README.md and branch2.md

```
$ git checkout -b branch1
$ git checkout -b branch2
$ git checkout branch1
$ touch branch1.md
$ git checkout branch2
$ touch branch2.md
```

Commit branch1 and branch2

```
$ git checkout branch1
$ git add .
$ git commit -m 'added branch1.md'
$ git checkout branch2
$ git add .
$ git commit -m 'added branch2.md'
```

Make changes to master's README and merge the change into branch1 and branch2:

```
$ git checkout master
$ vim README.md
# ...make some changes to README.md
$ git add .
$ git commit -m 'updated README.md'
```