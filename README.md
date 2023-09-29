# st-grav-flexipatch
st-flexipatch by bakkeby with my patches selected and some config fixes

## what are de 1 patches
- ALPHA (i like me them transparency)
- ANYSIZE_SIMPLE (works)
- BLINKING_CURSOR (cursor look cool)
- BOX_DRAW (my don font have good brail fonts :(
- COLUMNS (it sounded good
- DESKTOP-ENTRY (automatically was in flexipatch)
- FONT2 (yeah)
- LIGATURES (ligma balls)
- NETWMICON (icones)
- OPENURLONCLICK (clickity clack)
- SYNC (idk what this does)
- UNDERCURL (better than staight lines)
- USE_XFTFONTMATCH (actually also dont know what it does)
- VERTCENTER (dont understand but yeah)
- VIM_BROWSE (amazing, apart from the fact of no ctrl + {, and some other vim commands missing)
- VISUAL_BELL (visual bell is my lover) 
- WIDE_GLYPHS (plutin)
- XRESOURCES (allows for theme files, i like)
- XRESOURCES_RELOAD (change on the fly i very like)

## how 2 build if yo dumb
0. [dependers](https://github.com/siduck/st#dependencies)
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
so yeah it can include other files and shit
### apply themes while terminals are still on
you just do like and it kinda works
```
killall -USR1 st
```
so yeah you can do it at once too
```
xrdb <path> && killall -USR1 st &
```
- edit make yo own themes
go read theme files or something, go copy and make a new one, you can figure it out yourself 


### Might add
- CLIPBOARD Copy button does work ~~(websites with copy button do not transfer, but ctrl + c or rightclick prompt works)~~ 

> Some patches were selected not for need but it sounded cool. I could make another version with only essential patches but im lazy

Thanks to [bakkeby](https://github.com/bakkeby/st-flexipatch) and to [suckless](https://st.suckless.org/)
