# TMUX GUIDE

## Starting a Session

To start a new TMUX session, use the following command:

```
tmux 
`C-a d` -- to detach
tmux new -s session-name
```

### Session Management

TMUX provides several shortcuts for managing sessions:

- Create a new session: `C-a :new-session -s <session-name>`
- Switch to a specific session: `C-a s` (then use arrow keys to select session)
- Detach from the current session: `C-a d`
- Attach to a detached session: `tmux attach-session -t <session-name>`

Sessions in TMUX allow you to organize your work by separating different projects or tasks. You can create multiple sessions and switch between them easily.

To create a new session, use the `new-session` command followed by the `-s` option and the desired session name. For example, `C-a :new-session -s project-a` creates a new session named "project-a".

To switch between sessions, press `C-a s`. This will display a list of available sessions, and you can use the arrow keys to select the desired session.

If you need to detach from the current session and come back to it later, press `C-a d`. This will detach the session and return you to the regular shell. To reattach to a detached session, use the command `tmux attach-session -t <session-name>`. Replace `<session-name>` with the name of the session you want to reattach to.

Session management in TMUX allows you to keep your work organized and easily switch between different projects or tasks. It provides a convenient way to maintain separate working environments within a single terminal window.

## Basic Operations

- Split window horizontally: `C-a |`
- Split window vertically: `C-a -`
- Resize pane down: `C-a j`
- Resize pane up: `C-a k`
- Resize pane right: `C-a l`
- Resize pane left: `C-a h`
- Zoom in/out pane: `C-a m`
- Enable mouse support: `C-a + mouse`

### Closing Split Panes

To close a split pane in TMUX, follow these steps:

1. Enter the pane you want to close by selecting it with the arrow keys.
2. Press `C-a x` to close the selected pane.

### Exiting TMUX

To exit TMUX and close all sessions and windows, follow these steps:

1. Make sure you are not in a split pane. If you are, follow the steps above to close the split pane.
2. Press `C-a :` to enter the TMUX command prompt.
3. Type `kill-server` and press Enter. This will terminate the TMUX server and exit TMUX.

By following these steps, you can close split panes and exit TMUX effectively.

## Window Management

TMUX provides several shortcuts for managing windows:

- Create a new window: `C-a c`
- Close the current window: `C-a &`
- Switch to the next window: `C-a n`
- Switch to the previous window: `C-a p`
- Switch to a specific window: `C-a <window-index>`
- Rename the current window: `C-a ,`

To create a new window, press `C-a c`. This will open a new window in the current session. Each window acts as a separate workspace within the session.

To close the current window, press `C-a &`. Be aware that this will close the entire window and all panes within it.

To switch between windows, you can use the following shortcuts:

- `C-a n` to switch to the next window.
- `C-a p` to switch to the previous window.
- `C-a <window-index>` to switch to a specific window. Replace `<window-index>` with the index number of the window you want to switch to.

To rename the current window, press `C-a ,`. This will allow you to enter a new name for the window.

Window management in TMUX allows you to work on different tasks or projects simultaneously within a session. By creating and switching between windows, you can keep your work organized and easily access the desired workspace.

## Advanced Features

TMUX offers various features for developers, including:

- Session management
- Window management
- Pane management
- Session sharing and attaching
- Customizing keybindings and settings

TMUX offers the following advanced features for developers:

- **Session management**: TMUX allows you to create and manage multiple sessions. Each session can have its own set of windows and panes, making it easy to organize your work.
- **Window management**: Within each session, you can create multiple windows. Windows act as virtual terminals, allowing you to work on different tasks simultaneously.
- **Pane management**: TMUX allows you to split windows into multiple panes. This enables you to view and work on multiple terminals within a single window.
- **Session sharing and attaching**: TMUX allows you to share your session with other users, making it convenient for collaboration. You can also detach and reattach to sessions, allowing you to resume your work from where you left off.
- **Customizing keybindings and settings**: TMUX provides extensive customization options. You can define your own keybindings and configure various settings to suit your workflow and preferences.

These advanced features make TMUX a powerful tool for managing and organizing your terminal environment efficiently.