Menlo Patched for Powerline with Fixes
======================================

I always love using Menlo and wish there was better support for more font sizes. This version has been patched to work with Powerline with the symbols properly aligned and sized at smaller sizes (no more pixel gap) and the brackets () have been properly aligned at smaller font sizes.

OS X
-----

**1.** Double click the font in Find and select "Install this font." It will appear to have some very strange glyphs but will work as intended. 

**2.** If you use MacVim, add the following line to your `vimrc`:

```
set guifont=Menlo\ For\ Powerline
```

**3.** For use with Terminal.app or iTerm, change your settings according. You should select your font as `Menlo For Powerline`.

**4.** Enjoy!

Linux
-----

**1.** Copy `Menlo For Powerline.ttf` into your `~/.local/share/fonts` directory. (Or any X font directory)
```
$ cp "Menlo For Powerline.ttf" ~/.local/share/fonts
```

**2.** Update your fonts cache.
```
$ fc-cache -vf ~/.local/share/fonts
```
If you're in a terminal, you may or may not need to restart all windows before changes take effect.

**3.** If you use gvim, add the following line to your `vimrc`:

``` .vimrc
set guifont=Menlo\ For\ Powerline
```
**4.** For use with the terminal, change your settings according.

**5.** Enjoy!


Bold, Italic, Bold Italic
-------------------------

As far as I know, these extra font styles should work. I've had absolutely not problems with them, however, you may run into an issue. I added them as to provide support for bold, italic, and bold italic fonts within the terminal. Please let me know if you have any issues.


Airline/Powerline
------------------------
I have not tested this font with vanilla powerline, however, all the symbols work fine with the powerline oh-my-zsh theme.
If you use airline, add the following to your `vimrc`:

``` .vimrc
let g:airline_symbols = {}
let g:airline_left_sep = ''
let g:airline_left_alt_sep = ''
let g:airline_right_sep = ''
let g:airline_right_alt_sep = ''
let g:airline_symbols.branch = ''
let g:airline_symbols.readonly = ''
let g:airline_symbols.linenr = '☰'
let g:airline_symbols.maxlinenr = ''
let g:airline_symbols.whitespace = 'Ξ'
let g:airline_symbols.crypt = ''
let g:airline_symbols.paste = 'ρ'
let g:airline_symbols.notexists = '∄'
```
**NB:** Not all of these will be necessary on all systems

I do not know the process for vim powerline, however, it will be similar and the symbols should be the same.
