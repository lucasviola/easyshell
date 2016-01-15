---
title: "Custom Bash"
bg: mod-white
color: white
fa-icon: terminal
---

# Custom Bash

### Customize your bash cursor

The `PS1` environment variable contains the style for the bash cursor:

Export it to your ~/.bashrc file:


`export PS1='\u@\h \$'`

This will print the following as a cursor: `user@host $`

Some formatting options can be:

`\h - The hostname, up to the first ' . ' `

`\H - The hostname. `

`\n - A newline. `

`\t - The time, in 24-hour HH:MM:SS format. `

`\T - The time, in 12-hour HH:MM:SS format. `

`\@ - The time, in 12-hour am/pm format. `

`\u - The username of the current user. `

`\w - The current working directory, with $HOME abbreviated with a tilde (uses the $PROMPT_DIRTRIM variable). `

`\W - The basename of $PWD, with $HOME abbreviated with a tilde. `

Further reading:

[PS1 Generator](http://bashrcgenerator.com/)

[Git info on bash PS1](http://mediadoneright.com/content/ultimate-git-ps1-bash-prompt)

[Bash manual](http://www.gnu.org/software/bash/manual/bashref.html)
