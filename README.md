# vim-tid

A tiddler syntax file for the VIM editor.

This is a rough syntax file that need some tuning.  Please pull request.

## Installation

### Using the Vundle plugin manager

Add this to your `~/.vimrc` in the usual place.

    Plugin 'simonbaird/vim-tid'

Then install it like this:

    vim '+PluginInstall! vim-tid'

It should work just as well with other plugin managers. Consult the plugin
manager's documentation if you don't know what to do.

### Installing manually

Copy `syntax/tid.vim` into `~/.vim/syntax/`

Append the following lines your `.vimrc` file:

    au BufRead,BufNewFile *.tid set filetype=tid
    au! Syntax tid source ~/.vim/syntax/tid.vim

**Note:** You may need to turn on syntax highlighting via your `.vimrc` file:

    syntax on
