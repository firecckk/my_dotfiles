# Manage my dotfiles

## install on new machine

```
echo ".cfg" >> .gitignore

git clone --bare <remote-git-repo-url> $HOME/.cfg

echo "alias config='/usr/bin/git --git-dir=$HOME/.cfg/ --work-tree=$HOME'" >> $HOME/.bashrc

config config --local status.showUntrackedFiles no

config checkout
```


