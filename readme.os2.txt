This is the OS/2 build of version 1.8 (28-Jul-1999) of the JPEG to
PostScript converter / wrapper jpeg2ps by Thomas Merz. 

This build was made IBM OS/2 2.x and above, and has been supported by
helpful suggestions of Roger de Reus from Denmark.


Installation:
-------------

The archive contains besides the complete source tree (in src)

-rw-a--     7719 Aug  5 09:32 jpeg2ps.1            man page
-rwxa--    44164 Aug  4 19:53 jpeg2ps.exe*         compressed executable
-rw-a--    69636 Aug  4 19:55 jpeg2ps.exu          uncompressed executable
-rw-a--    14926 Jul 28 12:50 jpeg2ps.txt          jpeg2ps docs by TM
-rw-a--     1729 Aug  5 09:38 readme.os2           this file
drwx---        0 Aug  4 20:12 src/

Just unpack it in a directory of your choice, using e.g. the free InfoZip
unzip. Unless you want the sources, enter the following:

  unzip jpeg2ps2.zip -x src

There are two executables. The *.exe is LX compressed with LxLite and
will run on OS/2 Warp 3.x and above, but not on OS/2 2.x. Should you run
OS/2 2.x you can try to copy the uncompressed *.exu over *.exe and use
that.

Next, move the executable to a location in your PATH, and the docs to a
spot where you normally keep your documentation. If you have GNU man
installed, move jpeg2ps.1 in the location for /man/man1.

To run it you need to have the emx runtime system installed, which you
find on the site where this file was as emxrt.zip, or on the sites
ftp-os2.cdrom.com or ftp-os2.nmsu.edu or ftp.leo.org. Newer versions
than emx09c+ef2 should be fine. I tested this only on Warp 4, and there
it works. If there is a need for a version that runs standalone (i.e.
w/o emx installed) let me know and I consider throwing one in.


Where to find it:
-----------------

This file lives (hopefully) on:

* Hobbes:
 ftp://ftp-os2.nmsu.edu:/pub/incoming/jpeg2ps2.zip
 ftp://ftp-os2.nmsu.edu:/pub/os2/apps/graphics/convert/jpeg2ps2.zip

* Walnut Creek archive (cdrom.com):
 ftp://ftp-os2.cdrom.com/pub/os2/incoming/jpeg2ps2.zip

   and, despite a huge backlog, hopefully soon:

 ftp://ftp-os2.cdrom.com/pub/hobbes/graphics/jpeg2ps2.zip
 ftp://ftp.cdrom.com/pub/os2/graphics/jpeg2ps2.zip

* Comprehensive Tex Archive Network (CTAN, like ftp.dante.de + mirrors):
 CTAN:/pub/tex/ctan/graphics/jpeg2ps/jpeg2ps2.zip   or
 CTAN:/pub/tex/ctan/systems/os2/jpeg2ps/jpeg2ps2.zip
       tex-archive/support/jpeg2ps/os2/

* LEO (maybe):
 ftp://ftp.leo.org:/pub/comp/os/os2/leo/graphics/jpeg2ps2.zip


Sources:
--------

The original sources are from URL <http://www.ifconnection.de/~tm>. 

Build it yourself:
---------------
The executable was built from the unmodified sources with gcc
2.7.2.1.f.2 / emx09c + emxfix2 applied, calling
 
  make "CCFLAGS=-c -DA4 -DDOS -O2" "LDFLAGS=-s" "EXE=.exe"



More information & disclaimer:
------------------------------

For original information see the file jpeg2ps.txt. No warranties,
implied or explicit are given, you use the program at your own risk.


Have fun!         Stefan A. Deutscher (sad@utk.edu / stefand@ibm.net)


Version history of OS/2 port:
-----------------------------

*  4-Aug-1999:
   Build of version 1.8.

* 29-Jul-1997:
   Now a problem in the port with some files not being diplayed properly
   is fixed.

*  5-May-1997:
   First OS/2 version.


# eof.
