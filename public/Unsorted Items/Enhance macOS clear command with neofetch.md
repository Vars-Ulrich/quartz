---
title: 
tags:
  - tutorial
  - macOS
  - terminal
icon: 
aliases:
---
This will hopefully help you as it has helped me in keeping my terminal windows disciplined when using multiple shells/tmux.  When applied, each use of the `clear` command will also invoke `neofetch` giving a visually appealing and which-shell-indicative print-out every time you issue the command. 

We will also configure an alias called `clearall` which will invoke **only the original `clear` binary **

### 1. Install Homebrew and neofetch if you haven't already

#### Install Homebrew
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
https://docs.brew.sh/Installation
#### Use Homebrew to install neofetch
```bash
brew install neofetch
```

### 2.  Create or open your `.zshrc` file:
```bash
nano ~/.zshrc
```

### 3.  Paste this at the end of the file.
```bash
# enhance 'clear' command by subsequently invoking neofetch
# Redefine clear to run the system clear followed by neofetch
clear() {
    /usr/bin/clear  # Directly call the clear binary
    neofetch
}

# call original clear binary using "clearall"
alias clearall=/usr/bin/clear
```

### 4.  Save and exit the file
- ctl + o to write out.
	- press enter when prompted for a name.  It must be `.zshrc`
- ctl + x to exit nano

### 4. Set your newly saved file as your shell source:
```bash
source ~/.zshrc
```
