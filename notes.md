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