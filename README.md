



To make your VS Code work with Powerline fonts: 
1- download proper patched font - [Foked Here](https://github.com/abertsch/Menlo-for-Powerline)
2- In your User Settings (Code | Preferences | Settings) add this:
{
"terminal.integrated.fontFamily": "Menlo for Powerline",
}
And  your prompt in Code now looks right!

*Note*  this is for my own use only, and the credits go to the post here: *(with my thanks!)*
https://dev.to/mattstratton/making-powerline-work-in-visual-studio-code-terminal-1m7

(Yes, the colors look different than the previous screenshot; since taking those screenshots I changed from using the powerlevel9k oh-my-zsh theme to instead use powerline-go.)

Menlo for Powerline
===================

Menlo font patched to work with Powerline. Menlo's always been may favorite font to use on OS X while programming, but I was annoyed that I couldn't find a properly patched file anywhere. After a bit of trial and error, I managed to create a working version. If you find any errors with the font, please let me know.

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
