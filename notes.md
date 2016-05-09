git add
-------

add is a multipurpose command: it covers:

- staging [moving from untracked to tracked] an untracked file (e.g., a new, locally-created file)
- stage tracked files (e.g., a file that was already being tracked, but has since been modified)
- mark merge-conflicted files as resolved.

Note that if you make changes to a file, then add it, then make additional changes to that file before committing, git status will show that file twice: once in staged, ready to be committed (for the first set of changes that have been added), and another entry in unstaged (for the more recent changes subsequent to the git add command). If you were to commit now, you would commit just the first round of changes.



.gitignore
----------

see https://github.com/github/gitignore for examples of .gitignore files.


git remote
----------

lists the shortnames of each remote handle specified.

if you run it with the -v flag, you will also get the URLs for those shortnames.

To add a new remote:

```
git remote add <shortname> <url>
```

if you add the show command, you can see more information about a remote:

```
git remote show <remoteName>
```


git fetch
---------

Use to get data from remotes:

```
git fetch <shortname>
```

This differs from git pull in that a pull automatically merges the remote's data into the code you are working on. fetch will just download the data to your local repo (you can manually merge later).

git push
--------

Use to push your data upstream. Syntax is:

```
git push <remote[short]name> <branch-name>
```

This only works if you have write access to the upstream server, and nobody else has pushed in the meantime (in the latter case, you need to fetch the other person's pushed data and merge into yours before you do a push).


git tag
-------

Use this to add a version metadata tag to a particular point in history (e.g., a public release version).

To tag the current state:

```
git tag -a v1.4 -m "my version 1.4"
```

Note you can omit the -m and git will launch your standard editor to type in a longer tag message.


To tag a historical state:

```
git tag -a v1.2 <checksum>
```

Tags do not get automatically transfered on push. You can push a particular tag with:

```
git push origin <tagName>
```

Or you can transfer all tags by adding the --tags flag to the push command.

