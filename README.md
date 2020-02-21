stefan-peng dotfiles
====================

I use [thoughtbot/dotfiles](https://github.com/thoughtbot/dotfiles) and
stefan-peng/dotfiles together using [the `*.local` convention][dot-local].

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

    git clone https://github.com/stefan-peng/dotfiles.git $HOME/stefan-peng/dotfiles

Install:

    env RCRC=$HOME/stefan-peng/dotfiles/rcrc rcup

This will create symlinks for config files in my home directory.

I can safely run `rcup` multiple times to update.

What's in it?
-------------

[vim](http://www.vim.org/) configuration:

* [Gruvbox color scheme](https://github.com/morhetz/gruvbox)
  (optionally, install
  [Gruvbox theme for macOS Terminal.app](https://github.com/morhetz/gruvbox-contrib))
* [vim-easy-align](https://github.com/junegunn/vim-easy-align)
* [Vim Tmux Navigator](https://github.com/christoomey/vim-tmux-navigator)

[git](http://git-scm.com/) configuration:

* `l` alias for tight, colored, log output.
* My name and email.
