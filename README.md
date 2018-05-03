# ncurses-overkill

Mirror of 0verkill, a game made with ncurses. Thanks to [archive.org](https://web.archive.org/web/20170105060044/artax.karlin.mff.cuni.cz/~brain/0verkill), this project can be given a GitHub home. The rest of this README has been snagged from the original site.

<img width="500" height="157" src="https://github.com/inferno986return/ncurses-overkill/blob/master/0verkill.gif" alt=""/>

## What Is 0verkill
0verkill is bloody 2D action deathmatch-like game in ASCII-ART running under Linux, OS/2 and Windows.

Throw away Doom, Quake and Duke Nukem - 0verkill comes. Now you don't even need graphic mode if you wanna take a bloody deathmatch with your friends.

The ASCII art that has always fascinated you started to move finally. No one has ever thought that ASCII is an animable kind of art. Finally you can taste the original appearance of elaborate action in full 16 colors of your plain old text terminal. You never though that ASCII letters are capable of network-game action in such a massive manner.

No one ever connected gushing blood with that innocent ASII letters that were so utterly boring until short recently, when 0verkill was released.

## How It Began
In times of ZX Spectrum we were great fans of this cool computer. We enjoyed speccy 2D games like Jet Set Willy or Manic Miner. Nowadays we admire have Doom or Quake deathmatch with friends.

Because there aren't still many games under Linux, idea of a new game was born. We wanted to come with something new, with a new network game under Linux.

Deathmatch games are great fun (and mess too) so we decided to create a new deathmatch game. 3D deathmatch games are too common, too dowdy - the only way was a 2D game.

Graphics under Linux isn't still the best. There's lot of different cards, plenty of different systems. On PC there's SVGALib, you must have root permissions for older versions. There are X, but they're slow and bureaucratic and programming under X isn't the simplest (if you don't wanna use megabytes of uncompatible libraries).

The only uniform graphics under Linux is ASCII. And isn't 2D deathmatch game in ASCII a great idea?

Finally 0verkill was approved as my project on faculty so now I have time for writing it.

## 0verkill Features
* four types of gun
* grenades
* armor
* counting frags and deaths
* walking, running, jumping, shooting, creeping, walking up the stairs, climbing up and down ladders
* automatic weapon switching
* damage depending on distance and hit body part
* item respawning
* invisibility
* chat
* online help
* players respawning on random places
* boundless connecting/disconnecting during the game
* choice of 15 different colors of hero, choice of male/female hero
* ASCII-art graphics in full 16 color text mode
* client-server architecture
* client's motion prediction => decent running on slower lines
* raw keyboard
* simple level editor, but not very user friendly, currently only for initiates
* graphics editor
* top players list
* full X support
* experimental reaperbots
* multi level support
* lethal objects
* two levels done at this moment
* experimental 3D support (like stereogram)

## Requirements
### To run 0verkill on Linux you need:
* GNU make
* GCC
* text mode
* if you want to run 0verkill in X you need libX11 and optionally libXpm

It runs with any libc version. No other libraries than listed are needed.

### To run 0verkill on OS/2 you must have:
* EMX
* bash
* GNU unix utilities
* optionally Xwindow system

## Installation And Running

### Compiling on Linux
1. download the source code
2. type `tar xvfz 0verkill.tgz`
3. enter the 0verkill directory
4. type `configure` and `make`, binaries will be compiled
5. type `server` to start server, or `server <port number>` to determine port number (default port is 6666)
6. to join the game type `0verkill` or `0verkill <xsize> <ysize>` to explicitely set picture size (in characters)
7. if you're running X type `x0verkill` or `x0verkill [-d <display>] [-f <font>]`
8. select server address and port, your color and name
9. to learn controls press the H key (it toggles help window, even during the game)
10. press ENTER and enjoy!

### Compiling on OS/2
1. download and unpack sources
2. set paths to your programs:
3. SET HOSTTYPE=i586
4. SET MACHTYPE=i586-pc-os2
5. SET CONFIG_SHELL=d:/prg/gnu/bin/bash.exe
6. SET CC=d:/prg/emx/bin/gcc.exe
7. SET MAKE=d:/prg/emx/bin/make.exe
8. SET EMXOPT=-h100
9. run `configure` (or if you have X11 for OS/2 run `configure --with-x`)
10. run make
11. other steps are the same as in Linux version

## TODO
Here is partial list of things I'd like to do add to 0verkill:

* teleports
* better level editor
* listing older messages in chat
* sound

## Development
0verkill was developed on AMD K6-II/400 machine with 64MB of memory, Linux 2.2.12, 2.2.19 and 2.4.13-ac8, libc5 and libc6. It was tested on 10M ethernet network, 28.8k modem and 115200 home-made infrared link RONJA (now 10Mbit 625nm red).

**Does anybody want (know how) to write reaperbots?**

## Copying
0verkill is a free software, it can be modified and/or redistributed under terms of [GNU General Public License](https://www.gnu.org/copyleft/gpl.html).

## Bugs
All fatal bugs should have been eliminated. There also shouldn't be any compilation bugs. But of course bugs appear everywhere, so if you find some, let me know.

Please send bug reports, problems, ideas and comments to my address.

## Authors
* Idea: Karel Kulhavy
* Coding: Petr Kulhavy
* Level: Petr Kulhavy
* Graphics: Petr Kulhavy, Karel Kulhavy, Martin Pergel
* Female hero: Vince Weaver
* Icon: Marwin98
* AVI editor: Karel Kulhavy
* Design:	Petr Kulhavy
* Web page: Petr Kulhavy
* OS/2 port: Mikulas Patocka
* Windows port: Filip Konvicka
* Second level: Martin Pergel, Petr Kulhavy
* Smoke and special effects: Martin Pergel
