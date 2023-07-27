# git-alias

alias=!git config -l | grep alias | cut -c 7-
a=add
aa=!git add . && git add -u . && git status
ac=!git add . && git commit
br=branch
bra=branch -a
c=commit
ca=commit --amend --no-edit
cm=commit -m
cmn=commit -n -m
cf=commit --fixup
co=checkout
cob=checkout -b
master=checkout master
next=checkout next
develop=checkout develop
cp=cherry-pick
fp=fetch --prune
l=log --graph --oneline --decorate --all
ll=log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --all
lg=log --stat --abbrev-commit
lst=log --graph --decorate --oneline --abbrev-commit --all --name-status
changelog=log --pretty=format:'%s%n%b'
p=push
pf=push --force-with-lease
rbo=rebase --onto
rbmaster=!git co master && git up && git co - && git rebase master
rbi=rebase -i --autosquash
rba=rebase --autosquash
ok=rebase --continue
ss=show --stat
s=status
