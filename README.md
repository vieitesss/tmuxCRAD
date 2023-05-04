# tmuxCRAD

This file allows you Creating, Renaming, Attach and Delete (CRAD) your [Tmux](https://github.com/tmux/tmux) sessions. It uses [fzf](https://github.com/junegunn/fzf) to easily find any session.

https://user-images.githubusercontent.com/60654781/236276954-25b48127-4cab-40a5-a6e0-95446b225090.mp4

## Getting started

First install Tmux and fzf in your machine following the links above.

Then execute the next commands (1 by 1).

```shell
git clone https://github.com/vieitesss/tmuxCRAD
cp tmuxCRAD/tmuxcrad /some/directory/in/your/$PATH
rm -rf tmuxCRAD
```

After that, you can execute the script just as any other command in your terminal.

If you want to execute it through a key combination in Tmux, add one of the following examples to your `.tmux.conf`.

```conf
# if you want to use your prefix [<prefix>C-s]
bind-key C-s run-shell "tmuxcrad"

# if you don't want to use your prefix [C-s]
bind-key -n C-s run-shell "tmuxcrad"
```

Remember reloading your config if you edited it.

# Key combinations

| Key   | Action               |
|-------|----------------------|
| Enter | Attach to a session  |
| C-n   | Create a new session |
| C-d   | Delete a session     |
| C-r   | Rename a session     |

To change any key, just modify the script. Be sure you change every match of the key you don't like.
