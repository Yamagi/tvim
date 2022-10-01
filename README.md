# tvim

A simpler wrapper script to start a Vim inside a *modern*
terminal. Supported terminals are:
 1. alacritty
 2. gnome-terminal
The first terminal found in $PATH will be used.

Behaves more or less like gvim without being gvim. For
the best experience it's recommended to add the Terminus
plugin to Vim: https://github.com/wincent/terminus

Depending on personal preferences and the color scheme,
Vim should be configured with 'set termguicolors' and
support for "modern" terminal features like italics or
colored undercurls.

Neither alacritty nor gnome-terminal pass stdin to the
vim subprocess. Shell substitutions can be used to work
around that: `tvim <($command_with_output)`
