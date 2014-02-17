# Git Tutorial

## VCS and DVCS
----
CVS (Version control system), like subversion, has a central server. All users need to publish or update code from that. Version contorl function can not work without the server.

But for DVCS (Distributed version control system), like git, user can use version controlling on his local repository, without any server.

## Git Basic
----
Create a git repository is super easy.

```
# Create a git repository in current directory.
$ git init your-project-name

# Clone from a remote git repository
git clone remote-repo-url
```

Git supports many protocols:

```
http protocol:
	https://github.com/Mavlarn/git-tutorial.git
Git protocol:
	git@github.com:Mavlarn/git-tutorial.git
ssh protocol:
	ssh://[user@]host.xz[:port]/path/to/repo.git/
	[user@]host.xz:path/to/repo.git
```

Working Directory <-> Index

```
# Add changed file to index(staging area).
$ git add modified-file
$ git add .   # add all files

# Remove files from index, also delete in working directory
$ git rm file-name
# remove the file from index and keep the change in working directory
$ git rm --cached file-name
```


Git status:

Display the change between working directory and current HEAD commit.

```
$ git status
# On branch master
# Changes to be committed:
#   (use "git reset HEAD <file>..." to unstage)
#
#   new file:   test2.tmp
#
# Changes not staged for commit:
#   (use "git add <file>..." to update what will be committed)
#   (use "git checkout -- <file>..." to discard changes in working directory)
#
#   modified:   git-tutorial.md
#
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#   pic/
#   test.txt
```

Git diff:

Show changes between the working directory and the index.







