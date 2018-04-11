# Git Rebase

## 用 Rebase 合併

下 rebase 指令
```
git rebase -i xxxxxxx
```

開始編輯，把要合併的部份從 pick 改為 squash
```
pick xxxxxxx test1
s    yyyyyyy test2
s    zzzzzzz test3

# Commands:
#  p, pick = use commit
#  r, reword = use commit, but edit the commit message
#  e, edit = use commit, but stop for amending
#  s, squash = use commit, but meld into previous commit
#  f, fixup = like "squash", but discard this commit's log message
#  x, exec = run command (the rest of the line) using shell
#
# If you remove a line here THAT COMMIT WILL BE LOST.
# However, if you remove everything, the rebase will be aborted.
```

編輯新的 commit 資訊
```
rebase all commit
#
# test1
#
# test2
#
# test3
#
# Please enter the commit message for your changes. Lines starting
# with '#' will be ignored, and an empty message aborts the commit.
# Not currently on any branch.
# Changes to be committed:
#   (use "git reset HEAD <file>..." to unstage)
#
#       modified:   a.txt
#
```

push !!! 
```
git push -f
```

## 復原 Rebase

```
git reflog
git reset xxxxxxx --hard
```



