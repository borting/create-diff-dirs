# gen-old-diff
Generate old-school patch, a pair of folders containing original and changed files, from two git commits.

## Why use this
Although modern VCS, like git, suggest (and provide commands) to send diff in patch format, some tech companies/engineers still prefer to send diff in a pair of folders, one contains original files and the other contains changed files.
(The naming of the paired folders are also various, such as old/new, origin/patch, before/after, etc.)
This project provides a shell script to quickly generate such a old-school patch between two git commits.

## How to use this
```
$ gen-old-diff.sh commit-1 commit-2 dest-dir
```
* commit-1 & commit-2 are SHA-1 key of commits
* dest-dir is the path for saveing original and changed files in a pair of sub-folders, old and new.
