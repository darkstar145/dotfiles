darkstar145 dotfiles
====================

I use [thoughtbot/dotfiles](https://github.com/thoughtbot/dotfiles) and
darkstar145/dotfiles together using [the `*.local` convention][dot-local].

[dot-local]:
http://robots.thoughtbot.com/manage-team-and-personal-dotfiles-together-with-rcm

Requirements
------------

Install [Homebrew](brew.sh).

Install zsh.

    brew install zsh

Set zsh as my login shell.

    chsh -s /usr/local/bin/zsh

Install [rcm](https://github.com/mike-burns/rcm).

    brew tap thoughtbot/formulae
    brew install rcm

Install
-------

Clone thoughtbot dotfiles:

    git clone https://github.com/thoughtbot/dotfiles $HOME/thoughtbot/dotfiles

Clone personal dotfiles:

    git clone https://github.com/darkstar145/dotfiles.git $HOME/darkstar145/dotfiles

Install:

    env RCRC=$HOME/darkstar145/dotfiles/rcrc rcup

This will create symlinks for config files in my home directory.

I can safely run `rcup` multiple times to update.

What's in it?
-------------

[vim](http://www.vim.org/) configuration:

* [GitHub color scheme](https://github.com/acarapetis/vim-colors-github)
  (optionally, install
  [GitHub theme for macOS Terminal.app](https://github.com/paulfryzel/github-terminal-theme))
* [vim-easy-align](https://github.com/junegunn/vim-easy-align)
* [Vim Tmux Navigator](https://github.com/christoomey/vim-tmux-navigator)

[git](http://git-scm.com/) configuration:

* `l` alias for tight, colored, log output.
* My name and email.
