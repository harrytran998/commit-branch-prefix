# Git commit branch prefix

Clone của anh [huynhminhtufu](https://github.com/huynhminhtufu/commit-branch-prefix) :)) Vì có cái text in ra cuối cùng hơi khó chịu 👻

## Install

### Oh My Zsh Plugin

Clone repositories

```
git clone https://github.com/harrytran998/commit-branch-prefix.git $ZSH/plugins/commit-branch-prefix
```

Open zsh config to find plugins=(git)

```
nano ~/.zshrc
```

Update your plugins array:

```
plugins=(... commit-branch-prefix)
```

### Typical Bash

```
curl -s https://raw.githubusercontent.com/harrytran998/commit-branch-prefix/master/bash-install.sh | sudo bash /dev/stdin
```

## How to use

Name your branch like: feat/**TICKET-ID**/branch-description, where TICKET-ID is your ticket/issue ID you want to prefix your commits.

Then you can use:

```
git commit -m "Fix something"
```

It will actually commit "TICKET-ID Fix something" for you.

However, if your branch name is not named like above, the commit will not be prefixed.
