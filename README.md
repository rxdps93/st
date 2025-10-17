st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.

Applied Patches
---------------
> scrollback-ringbuffer:    st-scrollback-ringbuffer-0.9.2.diff
> scrollback-mouse:         st-scrollback-mouse-0.9.2.diff    
> anysize:                  st-anysize-20220718-baa718-baa9357.diff
> alpha:                    st-alpha-20240814-a0274bc.diff
> changealpha:              st-changealpha-20230519-b44f2ad.diff

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

