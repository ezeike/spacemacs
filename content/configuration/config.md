+++
title = "General"
author = ["Eric Nielson"]
draft = false
+++

Custom spacemacs config begins here. Modify your .spacemacs as shown below.
This will load the elisp code in a file called config.el and then execute
the function enielson/config. This function will load and execute the rest
of the configuration.

This approach minimizes the changes to your .spacemacs file.

```elisp
(defun dotspacemacs/user-config ()
  (load "/home/enielson/.config/home-manager/emacs/config.el")
  (enielson/config)
  (message "user-config complete"))
```
<div class="src-block-caption">
  <span class="src-block-number">Code Snippet 1:</span>
  .spacemacs configuration file
</div>

The configuration entry point in config.el:

```elisp
(defun enielson/config ()
  (interactive)

  (message "Executing enielson/config")

  (load "/home/enielson/.config/emacs/keybinds.el")
  (load "/home/enielson/.config/emacs/save-hooks.el")
  (load "/home/enielson/.config/emacs/deploy.el")
  (load "/home/enielson/.config/emacs/debug-replaces.el")
  (load "/home/enielson/.config/emacs/persp.el")
  (load "/home/enielson/.config/emacs/spacemacs-buffer.el")
  (load "/home/enielson/.config/emacs/hugo-servers.el")
  (load "/home/enielson/.config/emacs/gpt.el")
  (load "/home/enielson/.config/emacs/gptel-extensions.el")

```
<div class="src-block-caption">
  <span class="src-block-number">Code Snippet 2:</span>
  Configuration entry point
</div>


## Customizing Startup Buffer {#customizing-startup-buffer}

All of the code for this is stored in .emacs.d/core/core-spacemacs-buffer.el.
The function names all make sense, and are in plain English, so skim through
and find what you want to change. I want to get rid of the footer.
