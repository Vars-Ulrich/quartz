---
title: 
tags:
  - macOS
  - terminal
  - tutorial
icon: 
aliases:
---
<iframe width="560" height="315" src="https://www.youtube.com/embed/TfW72EnOm68?si=EyiktGzIf1Ib16Sp" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

This one is really simple and can be done in just a few seconds. 

### 1.  Create or open your `.zshrc` file:
```bash
nano ~/.zshrc
```

### 2.  Paste this at the end of the file.
```bash
#file/dir colorization mimicking linux
PS1="%{%F{033}%}%n%{%f%}@%{%F{green}%}%m:%{%F{yellow}%}%~%{$%f%}%  "
export CLICOLOR=1
export LSCOLORS=ExFxBxDxCxegedabagacad
```

### 3.  Save and exit the file

### 4. Set your newly saved file as your shell source:
```bash
source ~/.zshrc
```

### 5. Use `ls` to list your files and directory and bask in the glory of shell coloration
