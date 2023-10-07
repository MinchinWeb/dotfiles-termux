Dotfiles
========

These are machine-specific dotfiles, managed by [homeshick](https://github.com/andsens/homeshick).

Termux is a terminal emulator + environment, running as an app on Android.

See <https://github.com/MinchinWeb/dotfiles> for base configuration repo and installation instructions.

`tput` (required for *liquid prompt*) is available as park of the `ncurses-utils` package.

    pkg install ncurses-utils

This also includes configuration for ZSH, but that will need to be install separately:

    pkg install zsh
    git clone https://github.com/ohmyzsh/ohmyzsh.git ~/.oh-my-zsh
    git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
    chsh

And answer the prompt with `zsh`, and then start a new session.
