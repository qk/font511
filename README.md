# font511
5x11 bitmap font

Because I like Fixed Semi Condensed (aka 6x13), but wanted a smaller font, that was just as readable and unstylized but had the same character width/height ratio.

font511 doesn't leave vertical spacing between lines, so it's up to your terminal settings if you want to cram in as much text as possible (for programming) or slightly improve readability for continuous text by leaving 1px empty space between lines (for irc or latex).

To change linespace in URxvt add the following to your `~/.Xresources` file:

    URxvt.lineSpace: 0

Font511s adds 1 pixel extra horizontal space for better readability. Some characters extend into the extra space to make them more readable.

In font611 all characters extend into the extra space. The font ended up looking very much like FixedSemicondensed. In my opinion, font511s is the most readable of the bunch, so that's what I use most of the time.

# Installation

Download release, then proceed as follows:

## Windows

Right click font511.fon, click 'Install'.

## Linux

Create folder `~/.fonts`, copy font511.bdf into it, and run

    mkfontdir ~/.fonts
    mkfontscale ~/.fonts
    xset +fp ~/.fonts
    xset fp rehash
    fc-cache
    fc-cache -fv
