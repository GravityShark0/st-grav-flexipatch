# st-grav-flexipatch

st-flexipatch by bakkeby with my patches selected and some config fixes

## what are de 1 patches

- ALPHA
  > i like me them transparency
- ANYSIZE_SIMPLE
  > works
- BOLD_IS_NOT_BRIGHT
  > it seemed correct
- BOX_DRAW
  > (my don font have good brail fonts :()
- CLIPBOARD
  > i just realized its purpose
- DESKTOP-ENTRY
  > automatically was in flexipatch
- FONT2
  > yeah
- KEYBOARDSELECT
  > wanted to replace VIM_BROWSE cause it crashes all the time
- LIGATURES
  > ligma balls
- NETWMICON
  > icones
- REFLOW_PATCH
  > better??
- SIXEL
  > VISTUALS
- SYNC
  > idk what this does
- UNDERCURL
  > better than staight lines
- USE_XFTFONTMATCH
  > actually also dont know what it does
- VERTCENTER
  > dont understand but yeah
- WIDE_GLYPHS
  > plutin
- XRESOURCES
  > allows for theme files, i like
- XRESOURCES_RELOAD
  > change on the fly i very like

## how 2 build if yo dumb

0. [dependers](https://github.com/siduck/st#dependencies)

- including gd (build with png support)
- or just disable it in config.mk if you dont wanna

1. clone it lol

```
git clone https://github.com/GravityShark0/st-grav-flexipatch.git && cd st-grav-flexipatch
```

2. and go an build it and stuff

```
# make clean install
```

3. then hide your trace from the government

```
rm -fr * && rmdir ../st-grav-flexipatch
```

## how 3 use kinda

### shortcuts

- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Left</kbd> decrease font size
- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Right</kbd> increase font size
- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Home</kbd> reset font size to default
- <kbd>Shift</kbd> + <kbd>LMB</kbd> on a web link to open in browser (except when in like sshed into a tmux minecraft server)
- <kbd>Alt</kbd> + <kbd>C</kbd> enter vim history view

#### shortcuts you should probably already know or are never going to use

- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>C</kbd> copy
- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>V</kbd> paste
- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Y</kbd> copy and paste selected region
- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>O</kbd> increase opacity
- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd> decrease opacity

### set themes

uhhh like

```
xrdb merge <theme path>
```

so yeah it can include other files and shit, and also install xrdb if you havent

### apply themes while terminals are still on

you just do like and it kinda works

```
killall -USR1 st
```

so yeah you can do it at once too

```
xrdb <path> && killall -USR1 st &
```

### edit make yo own themes

go read theme files or something, go copy and make a new one, you can figure it out yourself

### Might add

> Some patches were selected not for need but it sounded cool. I could make another version with only essential patches but im lazy

Thanks to [bakkeby](https://github.com/bakkeby/st-flexipatch) and to [suckless](https://st.suckless.org/)

original README

```
st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.


Requirements
------------
In order to build st you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

```
