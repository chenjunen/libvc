# libvc

C vCard library.  Fork of libvc, part of the [Rolo](http://rolo.sourceforge.net/) project, which seems abandoned.

Original read me file provided in README.

## Compilation

    autoreconf -f -i
    ./configure
    make
    make install

Note: if making changes, use

    git update-index --assume-unchanged INSTALL

to avoid automatic changes to INSTALL making it into the git history.

## Changes from Original

Original code by Andrew Hsu <ahsu@users.sf.net>.

Some Debian patches by [Rafael Laboissiere's](https://anonscm.debian.org/cgit/users/rafael/deb-pkg/libvc.git/) applied.  These are the same selected for the Arch AUR distribution, by Jeff Mickey and Loui Chang.

* Manpage fix.
* Fields spanning several lines.
* Buffer overflow fix.
* vCard2 field name fix.

My own updates:

* Fast parsing of large vCards.
