# Git Alias 設定

可以透過`git config --list`查看 _~/.gitconfig_ 內的設定

### 好用的快速指令設定：

* git config --global alias.br branch
* git config --global alias.co checkout
* git config --global alias.cm commit
* git config --global alias.df "diff"
* git config --global alias.ft "fetch"
* git config --global alias.l "log --oneline --graph"
* git config --global alias.ls 'log --graph --pretty=format:"%h &lt;%an&gt; %ar %s"
* git config --global alias.last 'log -1 HEAD'
* git config --global alias.st status
* git config --global alias.ss "status -s"
* git config --global alias.visual '!gitk'

### 加上顯示顏色的範例：

git config --global alias.lg "log --graph --pretty=format:'%C\(bold red\)%h%Creset -%C\(yellow\)%d%Creset %s %Cgreen\(%cr\) %C\(bold green\)&lt;%an&gt;%Creset' --abbrev-commit --date=relative"



