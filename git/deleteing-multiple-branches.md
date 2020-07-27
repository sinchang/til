# Deleting Multiple Branches in Git

To delete many branches based on a specified pattern do the following:

1. Open the terminal, or equivalent.
2. Type in git branch | grep "<pattern>" for a preview of the branches that will be deleted.
3. Type in git branch | grep "<pattern>" | xargs git branch -D
   Replace the <pattern> with a regular expression to match your branch names and that’s it.

example: `git branch | grep 'jeff\/.*' | xargs git branch -D`

Ref: https://medium.com/@rajsek/deleting-multiple-branches-in-git-e07be9f5073c
