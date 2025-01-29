+++
title = "Hugo"
author = ["Eric Nielson"]
draft = false
+++

<https://gohugo.io/getting-started/quick-start/>
<https://ox-hugo.scripter.co/doc/source-blocks/>

<a id="code-snippet--hugo quickstart"></a>
```shell
hugo new site quickstart
cd quickstart
git init
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke
echo theme = \"ananke\" >> config.toml
```

<a id="code-snippet--hugo new post"></a>
```shell
hugo new posts/title.md
```

<a id="code-snippet--test"></a>
```shell
ls | head
```


## Org Mode Shortcuts {#org-mode-shortcuts}


### Create hugo post {#create-hugo-post}

, e e H h

| snippet |              |
|---------|--------------|
| sb      | source block |


## Using yassnippet {#using-yassnippet}


## Hugo Export Save Hook {#hugo-export-save-hook}

To automatically export the current buffer on save, put this somewhere in your init:

<a id="code-snippet--hugo auto export save hook"></a>
```elisp
(add-hook 'after-save-hook 'hugo-save-hook)
```

and define this:

<a id="code-snippet--hugo-save-hook"></a>
```elisp
(defun hugo-save-hook ()
  (when (string-match "org/howto" buffer-file-name)
    (org-hugo-export-to-md)))
```

org/howto is any string in the buffer-file-name you want to trigger on.


## Local Server {#local-server}

Run "hugo server" to run a local http server:

<a id="code-snippet--hugo server"></a>
```shell
hugo server
```
