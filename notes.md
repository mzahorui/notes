## zsh
mkdir ex{00..10}     // automatic directory range incement

alias <name>="<value>"     // expands on the beggining of the line
alias -g <name>="<value>"     // expands everyvere, g == global

## nvim
Super + s + /     // search in file


## tmux
bind n split-window -h "note"     // keybind shorcut run command in a new pane

bind n split-window -h "zsh -ic note"     // keybind shortcut run command in a new pane and stay in it; The -i flag makes zsh run as an interactive shell (loading .zshrc), and -c note executes your function.

tmux source-file ~/.tmux.conf     // source reload tmux config

## bear
bear -- make    // create json for clangd 

## dif
