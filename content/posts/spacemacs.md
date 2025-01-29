+++
title = "1 - Spacemacs"
author = ["Eric Nielson"]
draft = false
+++

<style>
.my-table th,
.my-table td {
    padding: 20px;
    color: red;
    text-align: left;
}
</style>

<https://out-of-cheese-error.netlify.app/spacemacs-config>


## Core {#core}

<style>.my-table table { width: 80%;  }</style>

<div class="ox-hugo-table my-table">
<div class="table-caption">
  <span class="table-number">Table 1:</span>
  Shortcut keys for compilation
</div>

| Keys      | Function         | Description                              |
|-----------|------------------|------------------------------------------|
| SPC c k   | kill-compilation | Kill current compilation                 |
| SPC SPC   |                  | M-x equivalent                           |
| SPC h d v |                  | Find a variables value and purpose       |
| SPC h d k |                  | Find a key bindings function and purpose |

</div>


### Searching <span class="tag"><span class="TEST">TEST</span></span> {#searching}

<div class="ox-hugo-table my-table">
<div class="table-caption">
  <span class="table-number">Table 2:</span>
  Shortcut keys for searching
</div>

| Keys    | Function | Description                             |
|---------|----------|-----------------------------------------|
| \*      |          | Highlight symbol in buffer (transient)  |
| SPC s p |          | search for string in all files          |
| SPC /   |          | search for string in all files          |
| SPC s P |          | search for object at point in all files |
| SPC \*  |          | search for object at point in all files |
| SPC p f |          | find a file in project                  |

</div>


#### Global Search and Replace {#global-search-and-replace}

Perform a search using helm (e.g. SPC s p) and then use C-c C-e to open a new buffer with all matching lines from all files.
This buffer can be edited like any other and when saved, emacs updates each line accordingly in each file.

<div class="ox-hugo-table my-table">
<div class="table-caption">
  <span class="table-number">Table 3:</span>
  Shortcut keys in helm search
</div>

| Keys    | Function | Description                                                             |
|---------|----------|-------------------------------------------------------------------------|
| C-c C-e |          | Open a new buffer with only matching lines. Can search and replace here |

</div>


### Buffer Management {#buffer-management}

ibuffer for buffer management


## New {#new}


#### Symbol Overlay {#symbol-overlay}

Highlight (overlay) symbols and keep them highlighted. Able to overlay
multiple symbols, replace symbols, jump between instances and switch focused
symbol.

<div class="ox-hugo-table my-table">
<div class="table-caption">
  <span class="table-number">Table 4:</span>
  Shortcut keys for symbol overlays
</div>

| Keys      | Function | Description                                 |
|-----------|----------|---------------------------------------------|
| SPC s o   |          | Overlay symbol at point                     |
| SPC s o r |          | Replace overlaid symbol, use y/n after this |
| SPC s O   |          | Unoverlay all symbols                       |

</div>


### Narrowing {#narrowing}

You can limit the buffer to only display a specific portion of the file.
All searches and edits will only affect the narrowed portion.

<div class="ox-hugo-table my-table">
<div class="table-caption">
  <span class="table-number">Table 5:</span>
  Shortcut keys for narrowing
</div>

| Keys    | Function | Description                               |
|---------|----------|-------------------------------------------|
| SPC n f |          | narrow the buffer to the current function |
| SPC n p |          | narrow the buffer to the visible page     |
| SPC n r |          | narrow the buffer to the selected region  |
| SPC n w |          | widen, i.e show the whole buffer again    |

</div>


## Other {#other}

<div class="ox-hugo-table my-table">
<div class="table-caption">
  <span class="table-number">Table 6:</span>
  Shortcut keys for development
</div>

| Keys         | Function     | Description                               |
|--------------|--------------|-------------------------------------------|
| SPC h d k    | describe-key | Find command bound to given key sequence  |
| &lt;F1&gt; w | where-is     | Find key for command                      |
| -            | deer         | Quick switch to deer in current directory |

</div>

<div class="ox-hugo-table my-table">
<div class="table-caption">
  <span class="table-number">Table 7:</span>
  Shortcut keys for messages
</div>

| Keys      | Function        | Description          |
|-----------|-----------------|----------------------|
| SPC w p m | popwin:messages | Open messages window |

</div>

<div class="ox-hugo-table my-table">
<div class="table-caption">
  <span class="table-number">Table 8:</span>
  Incoming shortcuts
</div>

| Keys    | Function | Description         |
|---------|----------|---------------------|
| SPC f R |          | Rename current file |

</div>


## Running elisp {#running-elisp}

Select a region of code and run

<a id="code-snippet--eval region"></a>
```elisp
, e r
```

SPC x o open link

C-c . style modes

SPC p l create project layout
SPC p t neotree
SPC p p switch project
SPC p b buffers in project

SPC e n next error
SPC e p previous error

SPC l l change/create layout
SPC l o custom layouts
SPC l a add buffer to layout
SPC l b layout buffers
SPC l TAB previous layout
SPC l s/L save/Load layouts

SPC k p paste
SPC a u undo tree visualize

SPC f s save buffer
SPC f
SPC s p search files in project
SPC p f find file in project
SPC b b buffer navigate
SPC '   shell

SPC f e d edit .spacemacs
SPC f e R reload .spacemacs

SPC j i jump to definition in buffer
SPC j I jump to definition in any buffer

M x Runs commands
-- eshell
-- rename-buffer

F3 to save helm search results

MARKDOWN:

SPC m c r Render

HELM:

C-n C-p next/prev line

ORG:

SPC p o TODOs for current project
t toggle status of todo items
T insert todo heading
SPC m l open at point. for links
SPC m h s make header subheader
SPC m h i make header insert below
SPC m h I make header insert above

Use \*s for indent level

SPC b Y

GIT:

SPC g &gt; show submodule prompt
SPC g b open a magit blame
SPC g f h   show file commits history
SPC g H c   clear highlights
SPC g H h   highlight regions by age of commits
SPC g H t   highlight regions by last updated time
SPC g I open helm-gitignore
SPC g s open a magit status window
SPC g S stage current file
SPC g m magit dispatch popup
SPC g M display the last commit message of the current line
SPC g t launch the git time machine
SPC g U unstage current file

/   evil-search
$   open command output buffer
c c open a commit message buffer
b b checkout a branch
b c create a branch
f f fetch changes
F (r) u pull tracked branch and rebase
gr  refresh
j   goto next magit section
C-j next visual line
k   goto previous magit section
C-k previous visual line
l l open log buffer
n   next search occurrence
N   previous search occurrence
o   revert item at point
P u push to tracked branch
P m push to matching branch (e.g., upstream/develop to origin/develop)
q   quit
s   on a file or hunk in a diff: stage the file or hunk
x   discard changes

-   on a hunk: increase hunk size
-   on a hunk: decrease hunk size

S   stage all
TAB on a file: expand/collapse diff
u   on a staged file: unstage
U   unstage all staged files
v or V  select multiple lines
y   magic-refs (show branches)
z z stash changes

M-x list packages. i to mark, x to execute mark

SPC b M move buffer to another window
SPC b m kill all other buffers
SPC m e b eval buffer
SPC m s send to REPL

SPC m d f set breakpoint in function
SPC m e s eval current symbol

SPC i s insert snippet
M-x **snippet** for other functions. by region.
, g u find reference

SPC c k kill compilation

(setq-default spacemacs-show-trailing-whitespace nil)
(setq spacemacs-show-trailing-whitespace nil)
