darkstar145 dotfiles
====================

I use [thoughtbot/dotfiles](https://github.com/thoughtbot/dotfiles) and
darkstar145/dotfiles together using [the `*.local` convention][dot-local].

[dot-local]:
http://robots.thoughtbot.com/manage-team-and-personal-dotfiles-together-with-rcm

Requirements
------------

Set zsh as my login shell.

    chsh -s /bin/zsh

Install [rcm](https://github.com/mike-burns/rcm).

    brew tap thoughtbot/formulae
    brew install rcm

Install
-------

Clone onto my laptop:

    git clone git://github.com/darkstar145/dotfiles.git $HOME/darkstar145/dotfiles

Install:

    env RCRC=$HOME/darkstar145/dotfiles/rcrc rcup

This will create symlinks for config files in my home directory.

I can safely run `rcup` multiple times to update.

What's in it?
-------------

[vim](http://www.vim.org/) configuration:

* [GitHub color scheme](https://github.com/acarapetis/vim-colors-github)

[git](http://git-scm.com/) configuration:

* `l` alias for tight, colored, log output.
* My name and email.
