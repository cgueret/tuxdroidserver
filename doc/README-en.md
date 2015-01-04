TuxDroidServer
==========================

Joel Matteotti - joel_DOT_matteotti_AT_free_DOT_FR

http://sourceforge.net/projects/tuxdroidserver/

1. COMPILE THE CODE
2. INSTALL THE UDEV RULE
3. REMOVE THE UDEV RULE

===========================

For more information, see the online wiki: http://sourceforge.net/p/tuxdroidserver/francais/Home/

1. COMPILE THE CODE:
------------------------

    ./configure
    make
    make clean

2. INSTALL THE UDEV RULE:
---------------------------------

** !! This step needs to be done as root !! **

For Fux (USB dongle TuxDroid) to be correctly recognized, you have to
add a rule to udev and restart udev.

You can do this with the following command:

    make install

This will copy the TuxDroid udev rule to the udev rules directory, 
and restart your udev service.


3. REMOVAL OF RULE UDEV:
------------------------------------

** !! This step needs to be done as root !! **

If you want to uninstall the udev rule you can do with the
following command:

    make uninstall

This will remove the TuxDroid udev rule file and restart your udev service.
