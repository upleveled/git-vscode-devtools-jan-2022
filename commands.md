# git commands

`git commit -v` ==> add commit message with changes in file (please do this your default)

`git diff` ==> show differences on non staged files

`git diff --staged` ==> show differences on staged files

`git add --patch` ===> allow you to staged small parts of a file

[cool article](https://paritosh-pundir.medium.com/take-control-of-your-commits-with-git-adds-patch-mode-2a5187590c3)
[git image](https://informaticaynadamas.com/wp-content/uploads/2020/02/Agregar-un-t%C3%ADtulo-1.jpg)

You can use the patch mode by adding -p or --patch after git add while adding the files for commit.

```
git add -p myFile.js
```

or

```
git add --patch myFile.js
```

After you run this command, git will prompt you with small pieces of the file, where you have made changes, asking you to perform the following actions. It represents every edited chunk or portion of the code as hunk.

- y — stage this hunk
- n — do not stage this hunk
- q — quit; do not stage this hunk or any of the remaining ones
- a — stage this hunk and all later hunks in the file
- d — do not stage this hunk or any of the later hunks in the file
- s — split the current hunk into smaller hunks this is a diff
- e — manually edit the current hunk
- ? — print help

---

- / — search for a hunk matching the given regex
- j — leave this hunk undecided, see next undecided hunk
- J — leave this hunk undecided, see next hunk
- k — leave this hunk undecided, see previous undecided hunk
- K — leave this hunk undecided, see previous hunk
- g — select a hunk to go to
