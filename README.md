# zsh_custom

My personal [omz][oh-my-zsh] custom directory (`$ZSH_CUSTOM`) for ZSH shell happiness.

## Installation

### Pre-reqs

Install [omz][oh-my-zsh]:

```zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

```zsh
# be sure to install oh-my-zsh first
export ZSH_CUSTOM="${ZSH_CUSTOM:-~/.oh-my-zsh/custom}"
rm -rfi "$ZSH_CUSTOM"
git clone git@github.com:mattmc3/zsh_custom.git "$ZSH_CUSTOM"
```

## Root directory

Per oh-my-zsh docs:

> You can put files here to add functionality separated per file, which will be ignored by git.
> Files on the custom/ directory will be automatically loaded by the init script, in alphabetical order.
> For example: add yourself some shortcuts to projects you often work on.

```zsh
brainstormr=~/Projects/development/planetargon/brainstormr
cd $brainstormr
```

## Plugins

Custom plugins go in the plugins folder. Oh-my-zsh allows overriding its plugins
or making new ones.

External plugins are as simple as doing a `git clone --depth 1`. A script for
downloading my favorite ones is in the bin/clone_plugins.sh script.

```zsh
$ZSH_CUSTOM/bin/clone_plugins.sh
```

## Themes

Custom themes go in the themes folder.

[omz]: https://github.com/robbyrussell/oh-my-zsh
