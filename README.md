# setup

What I do to set up a new Mac. These are mostly notes for myself.

**NOTE:** Most of these do not require admin privileges

~~note to self: maybe upload my `.zshrc`?~~ Check out [my dotfiles](https://github.com/ThatXliner/dotfiles)!

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

##### Poetry
Poetry (modified) from [docs](https://python-poetry.org/docs/#enable-tab-completion-for-bash-fish-or-zsh):

```bash
mkdir -p $ZSH_CUSTOM/plugins/poetry && poetry completions zsh > $ZSH_CUSTOM/plugins/poetry/_poetry
```

Then add the `poetry` plugin to your `.zshrc`

### Powerlevel10k

## Editors

### Atom

### VSCodium

### Vim

## Tools

### Pyenv

```bash
curl -sSf https://pyenv.run | bash
```

Then add the following to your `.zshrc` before the `source $ZSH/oh-my-zsh.sh`

```bash
export PYENV_ROOT="$HOME/.pyenv"
export PATH="$PYENV_ROOT/bin:/Users/bryanhu/.local/bin:$PATH"
eval "$(pyenv init --path)"
```

### Homebrew

```bash
mkdir homebrew && curl -L https://github.com/Homebrew/brew/tarball/master | tar xz --strip 1 -C homebrew
```

I forgot how I got the completions. Maybe add the `brew` plugin to your `.zshrc` (I didn't)?

Remember to add `~/homebrew/bin` to your `$PATH`, though.

### Poetry

### Git

### GPG

#### Admin-less

#### Easiest

### Git, GitHub, and GPG

## Misc

---

Helpful tips if you read this far:

 - [How to open and use apps downloaded from GitHub (or any other source) that is not code signed](https://docs.brew.sh/FAQ#the-app-cant-be-opened-because-it-is-from-an-unidentified-developer)
