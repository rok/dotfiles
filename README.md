## Dotfiles
===========

## Install
- `git clone git://github.com/rok/dotfiles.git ~/dotfiles`
- `~/dotfiles/install`

## VIM

### vimrc

* 2 spaces, no tabs
* incremental, case-insensitive search
* vertical split goes right, horizontal split goes below
* cursor keys for movement are disabled!

* `<CR>` - remove highlighting after search
* `<Space>` - toggle current fold
* `<C-j/k/h/l>` - switch between splits (no need to prepend `<C-w>`)
* `Q` - format lines

### File switching (Command-T)

* `<leader><leader>` alternates between two most recent buffers
* `<leader>t` - jump to file
* `<leader>F` - search in directory of current buffer
* `<leader>b` - search buffer list
* `<leader>gt` - search tags
* `<C-s>` - open the selected file in a new split window
* `<C-v>` - open the selected file in a new vertical split window
* `<C-t>` - open the selected file in a new tab
* `<C-j>` - select next file in the file listing
* `<C-k>` - select previous file in the file listing
* `<C-f>` - flush file cache

## Tmux

- `C-h/j/k/l` - switch to pane in the given direction
- `C-\\` - toggle between last active panes

Under tmux prefix `C-a`:

- `C-l` - clear terminal
- `S` - switch to a session that starts with given name, or switch to the last session if no name given
- `R` - source `~/.tmux.conf` after changes

Regular tmux keybindings:

    % vertical split
    " horizontal split
    ! break pane into new window
    c new window

    o select next pane
    { swap pane with previous
    } swap pane with next
    n next window
    p previous window
    ) next session
    ( previous session
    ; select previously active pane
    l select previously active window

    s interactive session & window browser
    w interactive window browser

    $ rename session
    , rename window

    : command prompt
    d detach
    f search text in open windows

    [ copy mode
    ] paste buffer
    # list buffers
    - delete buffer
