## zsh
mkdir ex{00..10}     // automatic directory range incement

alias <name>="<value>"     // expands on the beggining of the line
alias -g <name>="<value>"     // expands everyvere, g == global

## nvim
Super + s + /     // search in file

### substitution

/*PROJECT WIDE SUBSTITUTION*/
Super + SG (ripgrep) -> <pattern> -> Ctrl-Q (add to quick list)     // adds pattern to quicklist for project wide substitution
:cfdo %s/old_pattern/new_pattern/gc | update    // The cfdo command runs the substitution on each file in the quickfix list, gc asks for confirmation on each match, and update saves the modified buffers.
/*END*/

## tmux
/*PANE NAVIGATION AND MANIPULATION*/
{
    Prefix + { - Move the current pane left or up

    Prefix + } - Move the current pane right or down

    Prefix + Ctrl+o - Rotate all panes clockwise

    Prefix + Alt+o - Rotate all panes counterclockwise
}
/*END*/

bind n split-window -h "note"     // keybind shorcut run command in a new pane

bind n split-window -h "zsh -ic note"     // keybind shortcut run command in a new pane and stay in it; The -i flag makes zsh run as an interactive shell (loading .zshrc), and -c note executes your function.

tmux source-file ~/.tmux.conf     // source reload tmux config

## bear
bear -- make    // create json for clangd 

## dif

## git
git restore .       // removes all unsteged changes

## package management: dnf, rpm, flat etc.
rpm -ivh package-name.rpm       // i - install; v - verbose; h - hash progress bar
