+++
title = "Save Hook"
author = ["Eric Nielson"]
draft = false
+++

Running _lsp-format-buffer_ and _lsp-organize-imports_ are two functions that you'll want to run so often they should be save hooks.

These not only format your code and organize your imports, imports are automatically added and removed as necessary.

Use the before-save-hook,

<a id="code-snippet--before-save-hook"></a>
```elisp
(add-hook 'before-save-hook 'enielson-before-save-hook)
```

<a id="code-snippet--format and organize save hook"></a>
```elisp
(defun enielson-before-save-hook ()
 (when (string-match ".go\\'" buffer-file-name)
   (lsp-format-buffer)
   (lsp-organize-imports)))
```
