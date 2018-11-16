AGB_Hack version 1.5
Copyright (C) 2007 by Donnie Russell



AGB_Hack is based on RevivedHack 1.1,
an adaptation of Don G. Kneller's
PC Hack 3.61.

Level compression uses Markus Franz
Xaver Johannes Oberhumer's
miniLZO 1.08, a mini subset of the LZO
real-time data compression library.



History Of This Game
====================

[1984?] Hack by Jay Fenlason with help from Kenny Woodland, Mike Thome and Jon
        Payne.

       Inspired by Rogue, with twice as many monster types.

[1985] Hack 1.0.3 by Andries E. Brouwer.

       Evolution of Jay Fenlason's Hack, more than three times larger.

[1986] PC Hack 3.61 by Don G. Kneller.

       Hack 1.0.3 ported to MS-DOS, with new features and bugfixes.

[1987] NetHack project begins, organized by Mike Stephenson.

[2004] RevivedHack 1.1 by Donnie Russell.

       PC Hack 3.61 updated for modern operating systems, with color, sound
       effects, and bugfixes.

[2007] AGB_Hack 1.5 by Donnie Russell.

       RevivedHack 1.1 ported to the GameBoy Advance, with level compression,
       menus, graphical tiles, and bugfixes.



License
=======

The software contained in this archive is freeware, and may not be sold in any
form for any reason whatsoever. This software is provided to the end-user
"as is", and comes with no warranty of any kind. In no event shall the
copyright owner be liable for any damage that may result from the use of this
software.

This software may be redistributed provided that the original archive is
whole, intact, and unmodified. Only copies identical to the original
distribution archive available from my web site are authorized for
redistribution. Proper credit must be given to all people involved in the
creation of this software near the point of redistribution. Redistribution of
this software on cartridge media is strictly prohibited.



Getting Started
===============

When the initial screen appears the game will ask you to enter your name. You
can allow the game to pick a name for you by pressing the START button (Enter
key), or you can enter one with the key selector. Turn it on by pressing the L
button, then type your name by moving the cursor around the alphabet with the
directional buttons, pressing the B button on each letter. Press the L button
to turn the selector off. When the selector is off, pressing the B button
(Backspace key) moves the cursor back one space. Press the START button to
enter your name.

At this point, the game will seed a sequence of random numbers based on the
amount of time elapsed since startup. Hack's gameplay is influenced by the
year, day of the year, and time of day, which are set to random values in the
GameBoy Advance version.

Next, you can select the type of character you would like to play, or have one
chosen for you randomly. Move the arrow-shaped cursor using the directional
buttons to the character you want then press the Enter, B, or A button. Each
character has its own strengths and weaknesses, so choose carefully.

Use the directional buttons to move your character. To move diagonally, hold
down the SELECT button, select the direction, then release the SELECT button.
To run, hold down the START button, select the direction, then release the
START button. You can also release the SELECT/START button before releasing
the directional buttons.

Roguelike games such as Hack are typically played by entering commands with
a keyboard. Since the GameBoy Advance doesn't have a keyboard, two alternative
input methods are available.

The easiest method is to press the Start button (Enter key) to open the game
menu, which consists of two screens, for objects and actions. Press the Left
and Right directional buttons to switch between them. Objects listed on the
object menu are those which you are currently carrying. Selecting an object on
this menu brings up a list of things you can do with that object. Some actions
on the actions menu also work on objects, either in your inventory or on the
ground. Pressing the R button (Escape key) exits the menu.

The second method is more cumbersome but also more flexible. Commands can be
entered by "typing" them with the key selector. Consult the two in-game help
screens that list the available commands (accessed with the '?' command), and
the meaning of various symbols (the '/' command) for more information.

While playing, some game messages are too numerous to be displayed at once. To
continue viewing the following message(s), press the A button (Space key).

To cancel a command in progress, press the R button (Escape key).

Entering the '@' command with the key selector toggles the automatic picking
up of objects on or off. This setting is off by default. Gold is always picked
up if it is the only object at your current location.

To repeat the last command (for example, to fire another arrow), open the key
selector with the L button, move the cursor to the 'a' key (the "again"
command) and press the R button. Thereafter, pressing L then R repeatedly will
continue entering the same command.

At the bottom of the display, you can see what dungeon level you are on, how
many hit points you have now and will have when fully recovered, how much gold
you are carrying, what your armor class is (the lower the better), your
strength, experience level and the state of your stomach. Please note that in
graphical tile mode some status information may be obscured by the minimap.

If you ever find yourself inside a room with no exits, use the 's' (search)
command repeatedly along the walls of the room. This command can also be used
to find hidden traps. By default, the Select button is defined as 's'.

To quit the current game, enter the 'Q' command with the key selector, or
select "Quit" from the actions menu screen.



How Saved Games Work
====================

As you play AGB_Hack, each "keystroke" is recorded in a special area of memory
that is not erased when the power is turned off. Before ending a game session,
you should enter the command 'S' with the key selector to save and halt the
game, making it safe to turn off the power. If you accidentally turn off the
power without using this command first, there is a small chance that the saved
data will be corrupted.

To continue a previous game, turn on the console, and if a saved game is
found, it will be quickly played back to the point where you left off.



A Note About Memory
===================

There is a limited amount of memory available for saving games, enough
for 65,527 "keystrokes". Any input made after this limit is not recorded, but
the game will continue playing normally. In my own experience, this limit has
never been reached, even for winning games.

Also, in testing, I have found that the GameBoy Advance has enough memory to
store around 30 visited dungeon levels, which theoretically is enough for a
complete winning game. Levels are compressed when not in use, and since the
amount of compression varies with each level, this is a very rough estimate.

If you attempt to visit more than 30 levels, there is an increasing chance
that the game will run out of memory. When that happens the dungeon will
collapse, immediately ending the current game. However, you will still be able
to see your final score.



Controls
========


Buttons (key selector off)
--------------------------

A        Type Space key

B        Type Backspace key

L        Turn key selector on

R        Type Escape key (cancel command, close menu)

START    Type Enter key (open game menu when game is waiting for a command)
         When used with directional buttons: run in specified direction

SELECT   Type defined key, initially 's' (search command)
         When used with directional buttons: move in specified diagonal
         direction.


Buttons (key selector on)
-------------------------

A        Type Space key, keep key selector on

B        Type selected key, keep key selector on

L        Turn key selector off

R        Type selected key, turn key selector off

START    Type Enter key, turn key selector off

SELECT   Define selected key, initially 's' (search command)



--------------------------------------------------------------------------------------------
changes.txt:

==========
1.3 -> 1.4
==========

-------
Changes
-------

Menu command interface was added.

Graphics functions were optimized.

Removed "last_multi" so that "again" command always executes previous command
only once. This is to prevent, for example, repeated prompts for the object
and direction of the "throw" command after a count was used.

When "pick up" command is used, and gold and one item are at player's
location, pick up gold but ask before picking up item.

During saved game playback no sound effects are played and dungeon now
scrolls.

Key selector is positioned so as to avoid obscuring current position of
cursor.

First byte of SRAM is skipped due to incompatibility with some hardware.

----------
Bugs fixed
----------

If you are levitating, and zap a wand of digging downwards, you'll still fall
into the hole you make.

Reading a scroll of food detection while you are confused is supposed to
detect potions. What it actually does is detect potions, except that when
counting the number of potions to show, it still counts food. This can cause
problems when there are different numbers of potions and foods on the board.

A scroll of destroy armor fails to operate on your shield.

If you read a scroll of enchant weapon while confused, the program fails to
check to see if you're actually wielding a weapon, which means that you can
wield your armor and rustproof it with an enchant weapon scroll.

Enchant or damage weapon, read while confused, fail to check for plural in
stating what happens to the weapon.

There doesn't seem to be any limit on how many hit points your pet can have.
Therefore, the pet can get negative or zero hit points if it wraps around
(past 127).

Wielding a dead cockatrice is safe, even if you aren't wearing gloves. (Gloves
are still required to safely pick one up, though, and you can't remove the
gloves while wielding it.)

Eating a dead bat sets confusion to 50, instead of adding 50. If you are very
confused, eating the bat could conceivably reduce your confusion.

When you wield a dead cockatrice against monsters, you are told that they turn
to stone, but the monsters only leave normal corpses.

A long worm that dies without leaving a corpse fails to print the worm tooth
on the screen.

If you eat a lump of royal jelly and it increases your strength but does
nothing else that would change the status line, the program fails to update
the status line.

Doing an inventory of gold will produce the response "1 gold pieces" (instead
of piece) if you only have 1.

A cockatrice that hits another cockatrice turns it to stone. However, when
you hit a cockatrice with a cockatrice corpse nothing happens.

When you zap a wand of undead turning at a corpse to bring it back to life,
the corpse doesn't get erased from the screen.

A cancelled rust monster can still rust your helmet, though not your armor.
A scorpion cannot be cancelled.

If you are confused and read a scroll of fire, you are damaged by the scroll
catching fire and burning your hands even if you are fire resistant.

You are damaged by scrolls catching fire after being hit by dragon fire or
bouncing wands of fire even if you are fire resistant.

'M' character remains on SDOOR after mimic is killed.



==========
1.4 -> 1.5
==========

-------
Changes
-------

Graphical tile mode was added (on by default).

Sound effects were changed, and new ones were added.

Cursor now wraps around at top and bottom of menus.

----------
Bugs fixed
----------

Lockup in xmore() caused by docrt() calling cls() calling more() calling
xmore() infinitely because flags.toplin was set. Fixed by setting
flags.toplin to 0 before calling docrt().



--------------------------------------------------------------------------------------------
guide.txt:

The following is adapted from Don G. Kneller's PC Hack documentation.



A Guide to AGB_Hack
===================



Introduction
------------

The object of Hack is to descend into a dungeon to retrieve the Amulet of
Yendor and return to the surface with it. The Amulet is in the possession of
the Wizard of Yendor.

Your character
--------------

You can be one of several character classes when you start the game. Each
character starts with different attributes (strength, hit points) and a
different inventory of items (armor, weapons, etc). You should try the
different classes to see which is best for you. The class most likely to
survive the first few dungeon levels is probably the cave-person. However,
each class has its strong and weak points so you should try them all.

The status line
---------------

At the bottom of the screen is displayed information about your state of
being. You see the dungeon level you are on, how many hit points you have now
(and will have when fully recovered), what your armor class is (the lower the
better), your strength, experience level and the state of your stomach.

The little dog
--------------

You start Hack accompanied by a little dog (nameable with the 'C' command) who
can be very useful to you -- try not to kill him! Your dog will follow you --
if you carry tripe rations, he will follow you even better. Sometimes he gets
in your way. Either move around him, or wait (with the '.' command) until he
moves. If you want him to follow you to the next dungeon level, he must be on
a square next to you when you descend or ascend the stairs. Sometimes he gets
hungry and confused and hits you. You can feed him by throwing food at him
with the 't' command.

Your dog may get mad at you if you move to a different dungeon level without
taking him with you. Although he may not hit you, he won't help you either.
You'll have to appease him somehow.

Your dog is useful for his ability to fight and to pick up and carry objects.

Of course, your dog can be male or female; it makes no difference in the game.

The dungeon
-----------

The dungeon is a set of levels connected through stairways and trapdoors.
Each level is an interconnected system of rooms and corridors. The rooms have
doors that lead to the corridors. You must walk straight through a door -- no
diagonals allowed. Some doors (and some corridors) are hidden and you must
search for them (with the 's' command). Usually you must search several times,
so use a repeat count (e.g. '5s'). Some rooms are special and have no doors or
connecting corridors. There is a way to get in, though, but you will have to
find out how on your own.

The Wizard resides below the normal dungeon levels and can't be reached by
only taking the stairs.

Some rooms have special contents -- some are shops (but be aware that the
shopkeeper expects payment (the 'p' command) for the items you get there) and
some are zoos, full of interesting monsters. Some rooms are lit and you can
see the entire room, and some rooms are dark so you can see only the floor
near you.

Monsters
--------

To fight monsters, move to occupy the same square they are in. You can also
throw things at them, or zap them with wands. It is best to leave some
monsters alone.

Objects
-------

The objects you find may be enchanted (that's good) or cursed (that's bad) or
normal. Cursed items are generally less effective than normal and also, once
you have them on your body, they are impossible to remove unless you remove
their curse.

You use different objects in different ways:

       )  WEAPONS are wielded ('w') or thrown ('t').
          Some weapons are more effective when used together. For example, you
          get more effect by wielding a bow before throwing arrows. 'w-' means
          to wield nothing; i.e. be barehanded.

       [  ARMOR is worn ('W') and taken off ('T').
          You can wear more than one piece of armor, but there are some
          restrictions on the combinations. For example, you can only wear one
          suit of armor, but you can also wear an elven cloak over it.

       !  POTIONS are quaffed ('q').

       =  RINGS are put on ('P') and removed ('R').
          You can only wear two rings at a time, one on each hand. Also,
          wearing rings makes you use up more food, so use them sparingly.

       /  WANDS are zapped ('z').
          Some wands need a direction to be zapped in, but others do not.

       ?  SCROLLS are read ('r').

       (  TOOLS are applied ('A').
          For example, to use a whistle, you apply it.

Initially you will not know what the potions, rings, wands or scrolls do until
you use them. They will have names like "XIXIXI". Some of these objects are
identified as soon as you use them (for example, a scroll of light causes a
dark room to be lit).

Other objects have no noticeable effect. If it's not immediately obvious what
a scroll or potion does the first time you use it, you may be asked to give it
a name. Hack does this so that if you have an idea about what the object does
you can name it something appropriate so the next time you find it you will
know something about it. Whenever Hack asks for a name it is possible to use
<Backspace> to erase the previous character and <Esc> to quit without
supplying a name.

Using some objects gives a message like "You have a strange feeling for a
moment, but it passes". This means the object would have done something but
couldn't do it now (for example, some scrolls affect your weapon, but if
you're not wielding a weapon you'll get this message).

If you want to name an individual object, use the name command '!'. To name
all objects of a certain type, use the call command 'c'. For both commands
Hack will prompt you for the inventory letter of the object you want to name
or call. For example, if you put on a silver ring that has inventory letter
's' and notice that your strength increases by two, you might do this:
  
       'c' 's' 'strength' <Enter>
            (call all objects with the same type as item 's' "strength")
  
       '!' 's' '+2' <Enter>
            (call individual inventory item 's' "+2")
  
When you do an inventory you will see:
  
       s) a ring called strength named +2
  
The next time you pick up a silver ring it will be called strength so you will
know what it does. However, you will not know if it will increase or decrease
your strength! You will have to put it on to find out or you will have to
identify it.

Enchanting objects
------------------

If you enchant an object, it will be better than it was before. Enchanting
armor changes your armor class by 1 (e.g. you could go from class 7 to class 6
-- the less positive the number, the better the armor class. For weapons, the
more positive the number, the better. Thus a +2 mace is better than a +1 mace.
Some armor is better than others -- normal plate mail is better than normal
ring mail. Some weapons are better than others, but factors such as experience
and luck determine whether you can effectively use the better weapons.

Identifying objects
-------------------

The scroll of identify will help you to identify many objects, but generally
you just have to use them and see what happens. Occasionally a scroll of
identify will have the ability to identify several objects, so it is to your
advantage to have several unidentified objects before you use an identify
scroll. When you read a scroll of identify Hack will ask you which classes of
objects you want identified. If, for example, you choose rings and wands, then
for each ring in your pack you will be asked if you want to identify it. After
going through all the rings, you will be asked about the wands. If you do not
identify any of these objects you will return to the question about which
classes of objects you want identified.

The effect of rings may not be obvious, and cursed rings can't be removed
unless you remove their curse. Thus scrolls of identify are probably best used
to identify rings.

Scoring
-------

When the game ends, either by your death, when you quit, or if you escape from
the cave, Hack will give you a score. The scoring is based on many aspects of
your behavior but a rough estimate is obtained by taking the amount of gold
you've found in the cave plus four times your real experience. Precious gems
may be worth a lot of gold when brought to the exit. There is a 10% penalty
for dying.

What is "--More--"?
-------------------

Whenever there is a lot of information for you to see, Hack waits for you to
read it all by giving you a "--More--". If the "--More--" is displayed on the
normal response line (the top line that most messages are shown on), then Hack
is waiting for you to type the <Space> or <Enter> key.

If Hack has printed out a list of information (e.g. with the 'i' command),
then Hack will accept <Space> or <Enter> as well as the inventory letter of
anything in the list. Where is this useful? An example is when you want to
quaff a potion but you can't remember the letter of the potion you want. If
you type 'q' then '?', Hack will give you a list of all your potions
followed by a "--More--" message. If you type <Space> or <Enter> you will
return to the prompt about which potion you want to quaff. If you type the
inventory letter of the potion, you will immediately quaff that potion.

If the screen is completely cleared to give you information (e.g. you're
looking at the help documentation with the '?' command), then there will be
more than one screen full of information. In this case, <Space> or <Enter>
means "show the next screen" and 'q' or <Esc> means "stop".

Conclusion
----------

It may take hundreds of games before you discover all of Hack's secrets. The
only way to win is to learn how to reach the Wizard's domain. It will not be
easy, but with practice you might just be lucky enough to make it out of the
Dungeon alive with the Amulet!

--------------------------------------------------------------------------------------------
miniLZO_readme.txt:

-----BEGIN PGP SIGNED MESSAGE-----
Hash: SHA1


 ============================================================================
 miniLZO -- mini subset of the LZO real-time data compression library
 ============================================================================

 Author  : Markus Franz Xaver Johannes Oberhumer
           <markus@oberhumer.com>
           http://www.oberhumer.com/opensource/lzo/
 Version : 1.08
 Date    : 12-Jul-2002

 I've created miniLZO for projects where it is inconvenient to
 include (or require) the full LZO source code just because you
 want to add a little bit of data compression to your application.

 miniLZO implements the LZO1X-1 compressor and both the standard and
 safe LZO1X decompressor. Apart from fast compression it also useful
 for situations where you want to use pre-compressed data files (which
 must have been compressed with LZO1X-999).

 miniLZO consists of one C source file and two header files:
    minilzo.c
    minilzo.h
    lzoconf.h

 To use miniLZO just copy these files into your source directory, add
 minilzo.c to your Makefile and #include minilzo.h from your program.
 Note: you also must distribute this file (`README.LZO') with your project.

 minilzo.o compiles to about 6 kB (using gcc or Visual C on a i386), and
 the sources are about 14 kB when packed with zip - so there's no more
 excuse that your application doesn't support data compression :-)

 For more information, documentation, example programs and other support
 files (like Makefiles and build scripts) please download the full LZO
 package from
    http://www.oberhumer.com/opensource/lzo/

 Have fun,
  Markus


 P.S. minilzo.c is generated automatically from the LZO sources and
      therefore functionality is completely identical


 Appendix A: building miniLZO
 ----------------------------
 miniLZO is written such a way that it should compile and run
 out-of-the-box on most machines.

 If you are running on a very unusual architecture and lzo_init() fails then
 you should first recompile with `-DLZO_DEBUG' to see what causes the failure.
 The most probable case is something like `sizeof(char *) != sizeof(long)'.
 After identifying the problem you can compile by adding some defines
 like `-DSIZEOF_CHAR_P=8' to your Makefile.

 The best solution is (of course) using Autoconf - if your project uses
 Autoconf anyway just add `-DMINILZO_HAVE_CONFIG_H' to your compiler
 flags when compiling minilzo.c. See the LZO distribution for an example
 how to set up configure.in.


 Appendix B: list of public functions available in miniLZO
 ---------------------------------------------------------
 Library initialization
    lzo_init()

 Compression
    lzo1x_1_compress()

 Decompression
    lzo1x_decompress()
    lzo1x_decompress_safe()

 Checksum functions
    lzo_adler32()

 Version functions
    lzo_version()
    lzo_version_string()
    lzo_version_date()

 Portable (but slow) string functions
    lzo_memcmp()
    lzo_memcpy()
    lzo_memmove()
    lzo_memset()


 Appendix C: suggested macros for `configure.in' when using Autoconf
 -------------------------------------------------------------------
 Checks for typedefs and structures
    AC_CHECK_TYPE(ptrdiff_t,long)
    AC_TYPE_SIZE_T
    AC_CHECK_SIZEOF(unsigned short)
    AC_CHECK_SIZEOF(unsigned)
    AC_CHECK_SIZEOF(unsigned long)
    AC_CHECK_SIZEOF(char *)
    AC_CHECK_SIZEOF(ptrdiff_t)
    AC_CHECK_SIZEOF(size_t)

 Checks for compiler characteristics
    AC_C_CONST

 Checks for library functions
    AC_CHECK_FUNCS(memcmp memcpy memmove memset)


 Appendix D: Copyright
 ---------------------
 LZO and miniLZO are Copyright (C) 1996, 1997, 1998, 1999, 2000, 2001, 2002
 Markus Franz Xaver Johannes Oberhumer

 LZO and miniLZO are distributed under the terms of the GNU General
 Public License (GPL).  See the file COPYING.

 Special licenses for commercial and other applications which
 are not willing to accept the GNU General Public License
 are available by contacting the author.



-----BEGIN PGP SIGNATURE-----
Version: GnuPG v1.0.7 (GNU/Linux)

iD8DBQE9LPb4TWFXqwsgQ8kRAi/wAKCZ9Iej+voGhmKATaViOPS9chxGUwCgh5Dk
uwMS2PQ7BXHT0vf4yz+3tTc=
=PsNp
-----END PGP SIGNATURE-----



--------------------------------------------------------------------------------------------
miniLZO_copying.txt:

                    GNU GENERAL PUBLIC LICENSE
                       Version 2, June 1991

 Copyright (C) 1989, 1991 Free Software Foundation, Inc.
     59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 Everyone is permitted to copy and distribute verbatim copies
 of this license document, but changing it is not allowed.

                            Preamble

  The licenses for most software are designed to take away your
freedom to share and change it.  By contrast, the GNU General Public
License is intended to guarantee your freedom to share and change free
software--to make sure the software is free for all its users.  This
General Public License applies to most of the Free Software
Foundation's software and to any other program whose authors commit to
using it.  (Some other Free Software Foundation software is covered by
the GNU Library General Public License instead.)  You can apply it to
your programs, too.

  When we speak of free software, we are referring to freedom, not
price.  Our General Public Licenses are designed to make sure that you
have the freedom to distribute copies of free software (and charge for
this service if you wish), that you receive source code or can get it
if you want it, that you can change the software or use pieces of it
in new free programs; and that you know you can do these things.

  To protect your rights, we need to make restrictions that forbid
anyone to deny you these rights or to ask you to surrender the rights.
These restrictions translate to certain responsibilities for you if you
distribute copies of the software, or if you modify it.

  For example, if you distribute copies of such a program, whether
gratis or for a fee, you must give the recipients all the rights that
you have.  You must make sure that they, too, receive or can get the
source code.  And you must show them these terms so they know their
rights.

  We protect your rights with two steps: (1) copyright the software, and
(2) offer you this license which gives you legal permission to copy,
distribute and/or modify the software.

  Also, for each author's protection and ours, we want to make certain
that everyone understands that there is no warranty for this free
software.  If the software is modified by someone else and passed on, we
want its recipients to know that what they have is not the original, so
that any problems introduced by others will not reflect on the original
authors' reputations.

  Finally, any free program is threatened constantly by software
patents.  We wish to avoid the danger that redistributors of a free
program will individually obtain patent licenses, in effect making the
program proprietary.  To prevent this, we have made it clear that any
patent must be licensed for everyone's free use or not licensed at all.

  The precise terms and conditions for copying, distribution and
modification follow.

                    GNU GENERAL PUBLIC LICENSE
   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

  0. This License applies to any program or other work which contains
a notice placed by the copyright holder saying it may be distributed
under the terms of this General Public License.  The "Program", below,
refers to any such program or work, and a "work based on the Program"
means either the Program or any derivative work under copyright law:
that is to say, a work containing the Program or a portion of it,
either verbatim or with modifications and/or translated into another
language.  (Hereinafter, translation is included without limitation in
the term "modification".)  Each licensee is addressed as "you".

Activities other than copying, distribution and modification are not
covered by this License; they are outside its scope.  The act of
running the Program is not restricted, and the output from the Program
is covered only if its contents constitute a work based on the
Program (independent of having been made by running the Program).
Whether that is true depends on what the Program does.

  1. You may copy and distribute verbatim copies of the Program's
source code as you receive it, in any medium, provided that you
conspicuously and appropriately publish on each copy an appropriate
copyright notice and disclaimer of warranty; keep intact all the
notices that refer to this License and to the absence of any warranty;
and give any other recipients of the Program a copy of this License
along with the Program.

You may charge a fee for the physical act of transferring a copy, and
you may at your option offer warranty protection in exchange for a fee.

  2. You may modify your copy or copies of the Program or any portion
of it, thus forming a work based on the Program, and copy and
distribute such modifications or work under the terms of Section 1
above, provided that you also meet all of these conditions:

    a) You must cause the modified files to carry prominent notices
    stating that you changed the files and the date of any change.

    b) You must cause any work that you distribute or publish, that in
    whole or in part contains or is derived from the Program or any
    part thereof, to be licensed as a whole at no charge to all third
    parties under the terms of this License.

    c) If the modified program normally reads commands interactively
    when run, you must cause it, when started running for such
    interactive use in the most ordinary way, to print or display an
    announcement including an appropriate copyright notice and a
    notice that there is no warranty (or else, saying that you provide
    a warranty) and that users may redistribute the program under
    these conditions, and telling the user how to view a copy of this
    License.  (Exception: if the Program itself is interactive but
    does not normally print such an announcement, your work based on
    the Program is not required to print an announcement.)

These requirements apply to the modified work as a whole.  If
identifiable sections of that work are not derived from the Program,
and can be reasonably considered independent and separate works in
themselves, then this License, and its terms, do not apply to those
sections when you distribute them as separate works.  But when you
distribute the same sections as part of a whole which is a work based
on the Program, the distribution of the whole must be on the terms of
this License, whose permissions for other licensees extend to the
entire whole, and thus to each and every part regardless of who wrote it.

Thus, it is not the intent of this section to claim rights or contest
your rights to work written entirely by you; rather, the intent is to
exercise the right to control the distribution of derivative or
collective works based on the Program.

In addition, mere aggregation of another work not based on the Program
with the Program (or with a work based on the Program) on a volume of
a storage or distribution medium does not bring the other work under
the scope of this License.

  3. You may copy and distribute the Program (or a work based on it,
under Section 2) in object code or executable form under the terms of
Sections 1 and 2 above provided that you also do one of the following:

    a) Accompany it with the complete corresponding machine-readable
    source code, which must be distributed under the terms of Sections
    1 and 2 above on a medium customarily used for software interchange; or,

    b) Accompany it with a written offer, valid for at least three
    years, to give any third party, for a charge no more than your
    cost of physically performing source distribution, a complete
    machine-readable copy of the corresponding source code, to be
    distributed under the terms of Sections 1 and 2 above on a medium
    customarily used for software interchange; or,

    c) Accompany it with the information you received as to the offer
    to distribute corresponding source code.  (This alternative is
    allowed only for noncommercial distribution and only if you
    received the program in object code or executable form with such
    an offer, in accord with Subsection b above.)

The source code for a work means the preferred form of the work for
making modifications to it.  For an executable work, complete source
code means all the source code for all modules it contains, plus any
associated interface definition files, plus the scripts used to
control compilation and installation of the executable.  However, as a
special exception, the source code distributed need not include
anything that is normally distributed (in either source or binary
form) with the major components (compiler, kernel, and so on) of the
operating system on which the executable runs, unless that component
itself accompanies the executable.

If distribution of executable or object code is made by offering
access to copy from a designated place, then offering equivalent
access to copy the source code from the same place counts as
distribution of the source code, even though third parties are not
compelled to copy the source along with the object code.

  4. You may not copy, modify, sublicense, or distribute the Program
except as expressly provided under this License.  Any attempt
otherwise to copy, modify, sublicense or distribute the Program is
void, and will automatically terminate your rights under this License.
However, parties who have received copies, or rights, from you under
this License will not have their licenses terminated so long as such
parties remain in full compliance.

  5. You are not required to accept this License, since you have not
signed it.  However, nothing else grants you permission to modify or
distribute the Program or its derivative works.  These actions are
prohibited by law if you do not accept this License.  Therefore, by
modifying or distributing the Program (or any work based on the
Program), you indicate your acceptance of this License to do so, and
all its terms and conditions for copying, distributing or modifying
the Program or works based on it.

  6. Each time you redistribute the Program (or any work based on the
Program), the recipient automatically receives a license from the
original licensor to copy, distribute or modify the Program subject to
these terms and conditions.  You may not impose any further
restrictions on the recipients' exercise of the rights granted herein.
You are not responsible for enforcing compliance by third parties to
this License.

  7. If, as a consequence of a court judgment or allegation of patent
infringement or for any other reason (not limited to patent issues),
conditions are imposed on you (whether by court order, agreement or
otherwise) that contradict the conditions of this License, they do not
excuse you from the conditions of this License.  If you cannot
distribute so as to satisfy simultaneously your obligations under this
License and any other pertinent obligations, then as a consequence you
may not distribute the Program at all.  For example, if a patent
license would not permit royalty-free redistribution of the Program by
all those who receive copies directly or indirectly through you, then
the only way you could satisfy both it and this License would be to
refrain entirely from distribution of the Program.

If any portion of this section is held invalid or unenforceable under
any particular circumstance, the balance of the section is intended to
apply and the section as a whole is intended to apply in other
circumstances.

It is not the purpose of this section to induce you to infringe any
patents or other property right claims or to contest validity of any
such claims; this section has the sole purpose of protecting the
integrity of the free software distribution system, which is
implemented by public license practices.  Many people have made
generous contributions to the wide range of software distributed
through that system in reliance on consistent application of that
system; it is up to the author/donor to decide if he or she is willing
to distribute software through any other system and a licensee cannot
impose that choice.

This section is intended to make thoroughly clear what is believed to
be a consequence of the rest of this License.

  8. If the distribution and/or use of the Program is restricted in
certain countries either by patents or by copyrighted interfaces, the
original copyright holder who places the Program under this License
may add an explicit geographical distribution limitation excluding
those countries, so that distribution is permitted only in or among
countries not thus excluded.  In such case, this License incorporates
the limitation as if written in the body of this License.

  9. The Free Software Foundation may publish revised and/or new versions
of the General Public License from time to time.  Such new versions will
be similar in spirit to the present version, but may differ in detail to
address new problems or concerns.

Each version is given a distinguishing version number.  If the Program
specifies a version number of this License which applies to it and "any
later version", you have the option of following the terms and conditions
either of that version or of any later version published by the Free
Software Foundation.  If the Program does not specify a version number of
this License, you may choose any version ever published by the Free Software
Foundation.

  10. If you wish to incorporate parts of the Program into other free
programs whose distribution conditions are different, write to the author
to ask for permission.  For software which is copyrighted by the Free
Software Foundation, write to the Free Software Foundation; we sometimes
make exceptions for this.  Our decision will be guided by the two goals
of preserving the free status of all derivatives of our free software and
of promoting the sharing and reuse of software generally.

                            NO WARRANTY

  11. BECAUSE THE PROGRAM IS LICENSED FREE OF CHARGE, THERE IS NO WARRANTY
FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW.  EXCEPT WHEN
OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES
PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED
OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.  THE ENTIRE RISK AS
TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU.  SHOULD THE
PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING,
REPAIR OR CORRECTION.

  12. IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY AND/OR
REDISTRIBUTE THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES,
INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING
OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED
TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY
YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER
PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE
POSSIBILITY OF SUCH DAMAGES.

                     END OF TERMS AND CONDITIONS

            How to Apply These Terms to Your New Programs

  If you develop a new program, and you want it to be of the greatest
possible use to the public, the best way to achieve this is to make it
free software which everyone can redistribute and change under these terms.

  To do so, attach the following notices to the program.  It is safest
to attach them to the start of each source file to most effectively
convey the exclusion of warranty; and each file should have at least
the "copyright" line and a pointer to where the full notice is found.

    <one line to give the program's name and a brief idea of what it does.>
    Copyright (C) 19yy  <name of author>

    This program is free software; you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation; either version 2 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program; if not, write to the Free Software
    Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA


Also add information on how to contact you by electronic and paper mail.

If the program is interactive, make it output a short notice like this
when it starts in an interactive mode:

    Gnomovision version 69, Copyright (C) 19yy name of author
    Gnomovision comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
    This is free software, and you are welcome to redistribute it
    under certain conditions; type `show c' for details.

The hypothetical commands `show w' and `show c' should show the appropriate
parts of the General Public License.  Of course, the commands you use may
be called something other than `show w' and `show c'; they could even be
mouse-clicks or menu items--whatever suits your program.

You should also get your employer (if you work as a programmer) or your
school, if any, to sign a "copyright disclaimer" for the program, if
necessary.  Here is a sample; alter the names:

  Yoyodyne, Inc., hereby disclaims all copyright interest in the program
  `Gnomovision' (which makes passes at compilers) written by James Hacker.

  <signature of Ty Coon>, 1 April 1989
  Ty Coon, President of Vice

This General Public License does not permit incorporating your program into
proprietary programs.  If your program is a subroutine library, you may
consider it more useful to permit linking proprietary applications with the
library.  If this is what you want to do, use the GNU Library General
Public License instead of this License.


--------------------------------------------------------------------------------------------
