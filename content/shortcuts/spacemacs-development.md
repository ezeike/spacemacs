+++
title = "Shortcuts"
author = ["Eric Nielson"]
draft = false
+++

## Diffing {#diffing}

| Keys    | Description                        |
|---------|------------------------------------|
| M-0     | toggle focus treemacs              |
| SPC f t | toggle treemacs visibility         |
| SPC p t | toggle treemacs project visibility |
| SPC p a | switch between file and test file  |


## Extra {#extra}


### Treemacs {#treemacs}

| Binding   | Description                                                                                                                                    |
|-----------|------------------------------------------------------------------------------------------------------------------------------------------------|
| M-0       | Selected the treemacs window. Actually selects window #10, which is always assigned to treemacs.                                               |
| SPC 0     | Open treemacs in the current directory. When not visiting a file use $HOME as fallback. With a prefix arg manually select the root instead.    |
| SPC f B   | Find and select a bookmark. If it cannot be found rebuild view with the bookmark's location as root. Also open the bookmark with a prefix arg. |
| SPC f t   | Hide/show existing treemacs buffer. Create one for the current directory if no buffer exists.                                                  |
| SPC f T   | Manually focus the treemacs view on the currently selected file. Not needed when treemacs-follow-mode is enabled.                              |
| SPC f M-t | Manually focus the treemacs view on the currently selected file and tag.                                                                       |
| SPC p t   | Hide/show existing treemacs buffer. Add the current project to treemacs if not already added.                                                  |
| C-c C-p   | Add/remove/rename projects from treemacs                                                                                                       |

| Function | Description   |
|----------|---------------|
| SPC c l  | comment lines |

| Function              | Description   |
|-----------------------|---------------|
| treemacs-set-direcory | Set directory |
