## Closing tmux window

Tmux can often freeze up in a window. You will not be able to close the window by typing exit. This command can be used to kill an unresponsive tmux window

`tmux kill-window -t number_of_window`

Example: `tmux kill-window -t 0`
