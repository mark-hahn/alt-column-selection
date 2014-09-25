alt-column-selection
====================

A fork of sublime-style-column-select without the "sticky" problems.

When dragging the mouse and with the alt key pressed, this will select a rectangular region.  

This is a fork of @bigfive's "sublime-style-column-selection" Atom package, aka the project bigfive/atom-sublime-select in github, in that the core code was copied in the beginning of development.

# Motivation

@bigfive's package had the exact behavior I was used to from JetBrain's intelliJ IDEs.  (Contrary to the implication of @bigfive's package name many IDE's used this column selection technique).  I tried to use it but it had serious "stickiness" problems where the rectangular selection would not turn off.  It would also come on at random times. I and others posted issues but there has been no response to my issue after two months.  https://github.com/bigfive/atom-sublime-select/issues/17

# Philosophy

The "sublime-style-column-selection" code trusted browser events.  It trusted the alt-key to be down or up based on the history of keydown and keyup events.  It had several other similar assumptions.  This version has the opposite philosophy.  For example, if a mouseup or keyup event happens anywhere at any time in the entire workspace then selection is disabled.

# License

This version is copyright Mark Hahn using the MIT license.  See the LICENSE.md file.

The license for "sublime-style-column-selection" is included, in the attributions folder, as required by that license.

