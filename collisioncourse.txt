                             --------------------
                             | Collision Course |
                             --------------------

                          Version 1.0 (January 2006)

                             For GameBoy Advance

                         Programmed by Donnie Russell
                              Copyright (C) 2006



License
-------

The contents of this archive are freeware; they are not in the public domain.
This archive may only be redistributed in an unmodified state. The software
contained in this archive is provided to the end-user "as is", and comes with
no warranty of any kind. In no event shall the copyright owner be liable for
any damage that may result from the use of this software.

This software may not be sold in any form for any reason whatsoever.
Distribution of this software on cartridge media is strictly prohibited.



About This Game
---------------

This project started as a Spacewar/Asteroids-inspired game I wrote for MS-DOS
in the 1990's. Early in 2006 I decided to adapt it to the GameBoy Advance, in
the process rewriting much of the graphics code, and adding a few new
elements.



Technical Note
--------------

This game does not utilize any special graphics features of the GBA. Pixels
are simply written and cleared from the display (bitmap mode 3) in real-time,
fast enough to create the illusion of movement, and hopefully with little or
no flicker. As of this writing it has not been tested on hardware.



Status Information
------------------

The top-left side of the display shows your current score and up to five of
your reserve ships.



Controls
--------

Press START to begin a game of Collision Course.

Rotate your white triangular ship counterclockwise by pressing the left side
of the control pad, and right to rotate it clockwise. Apply forward thrust to
your ship by pressing the top side of the control pad. Your ship decelerates
when thrust is not applied.

Press the A button to fire your weapon at the green rocks floating around
your ship. Holding down the button causes your weapon to fire repeatedly.

Each large rock, when hit by your weapon, fragments into two medium-sized
rocks (20 points each), and each medium-sized rock into two small rocks (50
points each). Small rocks disintegrate completely (100 points each).

After all the rocks are destroyed, more will appear after a few seconds in the
areas indicated by the red arrows. Maneuver your ship out of the hazardous
areas before they appear.

At random times, a violet UFO will appear and begin shooting at rocks and your
ship. Destroying it is worth 500 points.

If your ship crashes or is destroyed by the UFO's weapon, you have two reserve
ships ready to replace it. For each 10,000 points you earn you will be
rewarded with a new reserve ship.

If your ship is destroyed, and you have no remaining ships, the game is over.
