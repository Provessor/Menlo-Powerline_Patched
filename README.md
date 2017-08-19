Menlo Patched for Powerline with Fixes
======================================

I always love using Menlo and wish there was better support for more font sizes. This version has been patched to work with Powerline with the symbols properly aligned and sized at smaller sizes (no more pixel gap) and the brackets () have been properly aligned at smaller font sizes.

OS X
-----

**1.** Double click the font in Find and select "Install this font." It will appear to have some very strange glyphs but will work as intended. 

**2.** If you use MacVim, add the following line to your `vimrc`:

```
set guifont=Menlo\ for\ Powerline
```

**3.** For use with Terminal.app or iTerm, change your settings according. You should select your font as `Menlo for Powerline`.

**4.** Enjoy!

Linux
-----

**NB:** I have not actually tried this, but it should work. I don't have access to a Linux machine, but these commands *should* be correct. 

**1.** Copy `Menlo for Powerline.ttf` into your `~/.fonts` directory. (Or any X font directory)
```
$ cp "Menlo for Powerline.ttf" ~/.fonts
```

**2.** Update your fonts cache.
```
$ fc-cache -vf ~/.fonts
```
If you're in a terminal, you may or may not need to restart all windows before changes take effect.

**3.** If you use gvim, add the following line to your `vimrc`:

```
set guifont=Menlo\ for\ Powerline
```

**4.** For use with the terminal, change your settings according.

**5.** Enjoy!


Bold, Italic, Bold Italic
-------------------------

As far as I know, these extra font styles should work. I've had absolutely not problems with them, however, you may run into an issue. I added them as to provide support for bold, italic, and bold italic fonts within the terminal. Please let me know if you have any issues.
