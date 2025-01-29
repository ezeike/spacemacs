+++
title = "Golang + Spacemacs"
author = ["Eric Nielson"]
draft = false
+++

<style>
.my-table th,
.my-table td {
    padding: 20px;
    text-align: left;
}
</style>


## Link {#link}


### [Golang Workflow on Youtube](https://www.youtube.com/watch?v=lvhIf3ynxgQ) {#golang-workflow-on-youtube}


## Shortcuts {#shortcuts}

<div class="ox-hugo-table my-table">
<div class="table-caption">
  <span class="table-number">Table 1:</span>
  Go Keys
</div>

| Keys    | Function                                                       | Description    |
|---------|----------------------------------------------------------------|----------------|
| , t t   | run current test                                               |                |
| , t p   | run all tests in file                                          |                |
| , t g f | generate tests for exported functions                          |                |
| , t g F | generate tests for all functions                               |                |
|         |                                                                |                |
| , r r   | lsp-rename                                                     | Renames object |
|         |                                                                |                |
| , h h   | godoc-at-point                                                 |                |
| K       | evil-smart-doc-lookup, seems to call godoc-at-point in go-mode |                |

</div>


## Save Hook {#save-hook}

Running _lsp-format-buffer_ and _lsp-organize-imports_ are two functions that you'll want to run so often they should be save hooks.

These not only format your code and organize your imports, imports are automatically added and removed as necessary.

<a id="code-snippet--format and organize save hook"></a>
```elisp
(defun enielson-before-save-hook ()
 (when (string-match ".go\\'" buffer-file-name)
   (lsp-format-buffer)
   (lsp-organize-imports)))
```
