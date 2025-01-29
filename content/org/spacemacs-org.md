+++
title = "Spacemacs Org Mode"
author = ["Eric Nielson"]
draft = false
+++

Links:

<https://web.archive.org/web/20210122070120/http://ehneilsen.net/notebook/orgExamples/org-examples.html#sec-2>

<https://zzamboni.org/post/beautifying-org-mode-in-emacs/>

<https://howardism.org/Technical/Emacs/orgmode-wordprocessor.html>


## Using mu4e with org mode {#using-mu4e-with-org-mode}

<https://www.djcbsoftware.nl/code/mu/mu4e/Org_002dmode-links.html>


### Can use `SPC a o l` to capture email link {#can-use-spc-a-o-l-to-capture-email-link}


### `C-c c` has been bound to `mu4e-org-store-and-capture`. Use it on headers or in an email {#c-c-c-has-been-bound-to-mu4e-org-store-and-capture-dot-use-it-on-headers-or-in-an-email}


#### New template has been added to create a todo from an email {#new-template-has-been-added-to-create-a-todo-from-an-email}


## Capturing {#capturing}

-   Use org-capture to capture something, it will go into refile.org
    -   todo marks the new entry with TODO
    -   todo from email marks the new entry with TODO and saves email info
    -   note tags the new entry with :NOTE:
    -   respond marks new entry with NEXT and adds a SCHEDULED property
    -   journal creates a timestamped entry in diary.org
    -   meeting marks new entry with MEETING, tags with :MEETING:
    -   phone marks new entry with PHONE, tags with :PHONE:
    -   habit marks new entry with NEXT and sets a repeat property


## Basics {#basics}

`C-RET` make new heading
`M-o` make new subheading below current heading


## Refiling {#refiling}

When ready process refile.org, use org-refile on entries and select where to send them. Targets are all files listed in org-agenda-files.


## Completing Tasks {#completing-tasks}


## In an org file {#in-an-org-file}

| Key            | Function                                                  | Description                                                     |
|----------------|-----------------------------------------------------------|-----------------------------------------------------------------|
| , ,            |                                                           | Set/modify tags                                                 |
| , ,            |                                                           | Toggle checkbox                                                 |
| , ,            |                                                           | Re-align table                                                  |
| , d s          | org-schedule                                              | Add/modify scheduled date. `alt h/l` to modify date in calendar |
| , s r          | org-refile                                                |                                                                 |
| , d d          | org-deadline                                              |                                                                 |
| , b e          |                                                           | Execute source block                                            |
| TAB            |                                                           | Collapse tree (toggle)                                          |
| C-c C-x o      | org-toggle-ordered-property                               | Toggle whether items must be checked off in order               |
| M-o            | org-insert-heading+org-metaright (new line, new sublevel) |                                                                 |
| C-RET          | org-insert-heading (new line, same level)                 |                                                                 |
| S-Right        | rotate TODO states                                        |                                                                 |
| M-S-RET        | org-insert-todo-heading                                   | When in a plain list, create an entry with a checkbox           |
| M-hjkl         |                                                           | Shift tree or move row up/down                                  |
| M-Right/Left   |                                                           | Shift tree                                                      |
| S-M-Right/Left |                                                           | In org-table, create or delete column                           |
| SPC o C        |                                                           | org-capture                                                     |
| SPC a o l      |                                                           | store link (store &amp; insert, same as copy &amp; paste)       |
| SPC m i l      |                                                           | insert link                                                     |


## Get into agenda {#get-into-agenda}

-   `SPC a o a` `org-agenda-list` Directly to default week view
-   `SPC a o o` `org-agenda` a menu presenting options before viewing agenda
-   `SPC a o o d` `org-agenda` View agenda but also show all NEXT entries (must configure this work org-agenda-custom-commands)
-   `SPC a o o n` `org-agenda` Only view next actions
-   `SPC a o o w` `org-agenda` Only view waiting actions


## Inside agenda {#inside-agenda}

| Key | Description                          |
|-----|--------------------------------------|
| C-v | Change day/week/fortnight/month/year |
| g r | refresh agenda view                  |
| ^   | Filter by same outline parent        |

Find tasks:
C-c /   sparse tree
C-c C-C exit sparse tree


## snippets: {#snippets}


#### sb {#sb}

<!--list-separator-->

-  source block

    | shortcut | function             |
    |----------|----------------------|
    | , b e    | execute source block |


## Column Mode {#column-mode}


### `C-c C-x C-c` org-column mode for table editing of org mode entries, {#c-c-c-x-c-c-org-column-mode-for-table-editing-of-org-mode-entries}


### `C-c C-c` to exit {#c-c-c-c-to-exit}


### e to edit cell {#e-to-edit-cell}


## Save Hook {#save-hook}

Save hook executes this


### `SPC x d w` delete-trailing-whitespace {#spc-x-d-w-delete-trailing-whitespace}


### `C-M-\` indent-region {#c-m-indent-region}


### org-lint {#org-lint}
