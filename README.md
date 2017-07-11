# Vim Enhancements

To record stuff from the terminal:
- register at https://asciinema.org
- `asciinema rec --title="vim tabularize" -w 0.5`
- when done: press enter -> you get a link, there you get the markdown for the recording.

## Tabularize

https://github.com/godlygeek/tabular

    Plugin 'gg/tabular'

[![asciicast](https://asciinema.org/a/ZhNTgNSwzEN3bRC8LZhsTAdyG.png)](https://asciinema.org/a/ZhNTgNSwzEN3bRC8LZhsTAdyG)

## Correctly Indented Breakpoint

    let mapleader = ","
    map <Leader>b Oimport pdb; pdb.set_trace()<C-c>

hitting `,b` inserts a breakpoint the line above, correctly indented, no
matter where you are with the cursor:

[![asciicast](https://asciinema.org/a/LCx3dt7uOT7HmwLvF742Mtv6Q.png)](https://asciinema.org/a/LCx3dt7uOT7HmwLvF742Mtv6Q)


## Wrapping try-except around a problematic line

    map <Leader>e Otry:<Esc>j^i<TAB><Esc>oexcept Exception as ex:<CR>import pdb;pdb.set_trace()<Esc>^

hitting `,e`:

[![asciicast](https://asciinema.org/a/MzMg0nExfS3mtQTP4wZhTyEr9.png)](https://asciinema.org/a/MzMg0nExfS3mtQTP4wZhTyEr9)


## General Tips

### Pastemode

Use neovim - it is automatically going to pastemode at inserts.
Or [this](https://coderwall.com/p/if9mda/automatically-set-paste-mode-in-vim-when-pasting-in-insert-mode) (did not try though)



