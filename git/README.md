# GIT alias
1.  git config --global alias.ch checkout
2.  git config --global alias.c commit
3.  git config --global alias.st status
4.  git config --global alias.undo 'reset --soft HEAD~1'
5.  git config --global alias.amend '!git log -n 1 --pretty=tformat:%s%n%n%b | git commit -F - --amend'
6.  git config --global alias.tree 'log --graph --pretty=format:'%C(yellow)%h%C(cyan)%d%Creset %s %C(white)- %an, %ar%Creset''
7.  git config --global alias.review= '"!f() { git fetch origin pull/$1/head:pr/$1 && git checkout pr/$1; }; f"'