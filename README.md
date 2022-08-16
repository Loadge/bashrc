# About
This is the bashrc I like to setup in my machine when I enter a company.

To set it up, execute ```nano ~/.bashrc```

Then, paste:

```bash
# Daily Operations
alias g="git"
alias gt="git status"
alias gf="git fetch; git status"
alias ga="git add"
alias gdf="git diff"
alias sbash="source ~/.bashrc"
alias cdrepo="cd /c/Users/Loadge/Documents/workspace"

# Common stuff
alias ".."="cd .."
alias cd..='cd ..'
alias ls='ls --color=auto'
alias grep='grep --color=auto'
alias egrep='egrep --color=auto'
alias fgrep='fgrep --color=auto'
alias mkdir='mkdir -pv'
alias diff='colordiff'
alias path='echo -e ${PATH//:/\\n}'
alias now='date +"%T"'
alias nowtime=now
alias nowdate='date +"%d-%m-%Y"'
alias chown='chown --preserve-root'
alias chmod='chmod --preserve-root'
alias chgrp='chgrp --preserve-root'
alias apt-get="sudo apt-get"
alias reboot='sudo /sbin/reboot'
alias poweroff='sudo /sbin/poweroff'
alias halt='sudo /sbin/halt'
alias shutdown='sudo /sbin/shutdown now'
alias df='df -H'
alias du='du -ch'

## pass options to free ##
alias meminfo='free -m -l -t'

## get top process eating memory
alias psmem='ps auxf | sort -nr -k 4'
alias psmem10='ps auxf | sort -nr -k 4 | head -10'

## get top process eating cpu ##
alias pscpu='ps auxf | sort -nr -k 3'
```

Save it, then execute ```source ~/.bashrc```