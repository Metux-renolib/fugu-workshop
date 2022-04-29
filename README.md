# fugu-workshop
workshop repository for fugu


summary du workshop:

- cloner le repo du projet
- harmoniser sa configuration de github ($HOME/.gitconfig)
- trunk based vs feature branch
- git pull --rebase 
- git merge
- résolution de conflits
- rebase interactif avec pour squash ses commits




hello fugu, on va modifier cette ligne de code chacun de son côté pour générer des conflits :)

Georges
abdel
Can
mete
dihia
Syphax

url to documentation of git-config: 
https://git-scm.com/docs/git-config

prettier logging alias to put in your .gitconfig

[alias]

        lol = log --pretty=format:'%C(yellow)%h%Creset %C(green)%ad%Creset | %s %C(blue)%d%Creset %C(red)[%an]%Creset' --graph --date=short --color

A mettre dans le $HOME/.bashrc pour avoir le nom de la branche dans le shell:

parse_git_branch() {
     git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/ (\1)/'
}

info à stash
