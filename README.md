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

### File switching (CtrlP)

* `<leader><leader><Esc>` alternates between two most recent buffers
* `<leader>t` - jump to file

#### Once CtrlP is open:

* `<F5>` - purge the cache for the current directory to get new files, remove deleted files and apply new ignore options.
* `<c-f>`, `<c-b>` - cycle between modes.
* `<c-d>` - switch to filename only search instead of full path.
* `<c-r>` - switch to regexp mode.
* `<c-j>`, `<c-k>` - navigate the result list.
* `<c-t>` or `<c-v>`, `<c-x>` open the selected entry in a new tab or in a new split.
* `<c-n>`, `<c-p>` select the next/previous string in the prompt's history.
* `<c-y>` create a new file and its parent directories.
* `<c-z>` mark/unmark multiple files and `<c-o>` to open them.

### NERDTree

* `<F2>` - toggles NERDTree pane
* `<i>` - opens file in horizontal split
* `<s>` - opens file in vertical split

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
