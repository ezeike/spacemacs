+++
title = "Layouts, Perspectives & Projects"
author = ["Eric Nielson"]
draft = false
+++

## Definitions {#definitions}

A layout in Spacemacs is a sub-set of open buffers. It is convenient to use
one layout per project. If you do this then you can think of layouts as
"project layouts". A workspace is an arrangement of some number of buffers
within a layout. You can think of workspaces as "views into projects". For
example, a workspace is a specific set of buffers related to a task or area of
the project.


## Workflows {#workflows}

  Access layouts with `SPC l`
  From here, create and switch to different layouts (projects).
  Within these layouts (projects), workspaces exist. `SPC l w` to manage these.
Example:


## layout: middleware {#layout-middleware}


### workspace: metrics {#workspace-metrics}


## Shortcuts {#shortcuts}

<div class="ox-hugo-table my-table">
<div class="table-caption">
  <span class="table-number">Table 1:</span>
  Shortcut keys for development
</div>

| Keys    | Function                | Description                                             |
|---------|-------------------------|---------------------------------------------------------|
| M-0     |                         | toggle focus treemacs                                   |
| SPC f t |                         | toggle treemacs visibility                              |
| SPC p t |                         | toggle treemacs project visibility                      |
| SPC p a |                         | switch between file and test file                       |
| SPC p l |                         | list all projects                                       |
| SPC p b |                         | helm buffers in current project                         |
| SPC p k | projectile-kill-buffers | kill all buffers in project                             |
| Key     |                         | Description                                             |
| SPC l   |                         | layout transient state                                  |
| SPC l w |                         | workspace transient state                               |
| SPC b b |                         | lists all open buffers, default layout has global scope |
| SPC l b |                         | list buffers in current layout                          |
| SPC l a |                         | add buffer to current layout                            |
|         |                         |                                                         |
| SPC l x |                         | kills layout, buffers stay open                         |
| SPC l d |                         | close current layout                                    |
| SPC l l |                         | select or create layout by typing name                  |
| SPC l L |                         | load perspective                                        |
| SPC l   |                         | select layout                                           |
| SPC h l |                         | spacemacs-layouts help                                  |

</div>
