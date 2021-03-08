# setup

What I do to set up a new Mac. These are mostly notes for myself.

**NOTE:** Most of these do not require admin privileges


## Terminal and Shell

### iTerm2

1. Download the latest version of iTerm2 [here](https://iterm2.com/downloads.html).
2. Move it to `~/Applications`
3. Configure:

#### Configuration

* Install [snazzy theme](https://github.com/sindresorhus/iterm2-snazzy) and use it on the default profile
* Set theme to minimal (`Preferences > Appearence > Theme > Minimal`)
* Set `Preferences > General > Startup` to
![](./iterm_general_startup.png)
 * Set `Preferences > Profiles` to look like
![](iterm_profiles.png)
and
![](iterm_profiles_working_dir_adv_conf.png)
 * Turn off transparency in `Preferences > Profiles > iTerm2 > Window`
 * Set stuff:
![](iterm_epic_term.png)
![](iterm_epic_keys.png)
 * You're done I think

### Oh-my-zsh

* Curl-bash this:
```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

**Editing `~/.zshrc`:**

* Set the `COMPLETION_WAITING_DOTS` to `true`
* Export `UPDATE_ZSH_DAYS` to `13`

#### Plugins
 - git
 - brew
 - nvm
 - npm
 - pip
 - pyenv
 - python
 - invoke (CUSTOM!!!!)
 - poetry (CUSTOM!!!!)
 - colored-man-pages
 - ripgrep
 - z ([Install](#z))
 - zsh-autosuggestions ([Install](#zsh-))
 - zsh-syntax-highlighting ([Install](#zsh-))

##### z
Z is now [built-in](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/z). No install :smiley:!

##### zsh-*

##### Poetry and Invoke
Poetry (modified) from [docs](https://python-poetry.org/docs/#enable-tab-completion-for-bash-fish-or-zsh):

```bash
mkdir -p $ZSH_CUSTOM/plugins/poetry && poetry completions zsh > $ZSH_CUSTOM/plugins/poetry/_poetry
```

Invoke:
```bash
mkdir -p $ZSH_CUSTOM/plugins/invoke && invoke --print-completion-script=zsh > $ZSH_CUSTOM/plugins/invoke/_invoke
```

### Powerlevel10k

## Editors

### Atom

### VSCodium

### Vim

## Tools

### Pyenv

### Homebrew

### Poetry

### Git

### GPG

#### Admin-less

#### Easiest

### Git, GitHub, and GPG

## Misc
