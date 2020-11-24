---
description: >-
  Anaconda is installed with bash, so you may run into problems using conda if
  your OS shell is zsh. Here are some solutions:
---

# Anaconda with zsh

### 1. Append path to .zsh

Open .bash\_profile from terminal:

```text
$ open ~/.bash_profile
```

Copy snippet after  `>>> conda initialize >>>`. Open .zshrc:

```text
$ open ~/.zshrc
```

Paste the snippet at the bottom and save. Restart terminal. 

### 2. Switch to bash 

Although not a satisfying solution, you could temporarily switch to bash when you are using Anaconda.

```bash
# Switch to bash
$ chsh -s /bin/bash
# Switch back to zsh
$ chsh -s /bin/zsh
```

### Go back to previous page:

{% page-ref page="using-navigator/" %}

{% page-ref page="using-terminal.md" %}

