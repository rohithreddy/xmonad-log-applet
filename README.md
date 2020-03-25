# xmonad-log-applet

xmonad-log-applet is for Xmonad users who find the GNOME, MATE, or Xfce panel
useful. The applet will show the active workspaces, the title of the selected
window or whatever information you send it from your xmonad.hs.

xmonad-log-applet was originally written by Adam Wick, you can get more details
on the [old website][0].

## ChangeLog 

has been modified to work with libmatepanelapplet-4.0 


## Installation

There are two pieces of setup you'll need to get this working, assuming you are
already running Xmonad within [GNOME][1], MATE or [Xfce][2]:

* An xmonad.hs setup file that will send properly-formatted information to
  D-Bus. You can use [this xmonad.hs][3] as an example; obviously, feel free to
  change the colours to match your tastes.

* The panel applet. You can either get the current stable build as a
  [tarball][4], or pull the latest version from the git repository: `git clone
  git://github.com/alexkay/xmonad-log-applet.git`

The applet supports GNOME 2, GNOME 3, MATE and Xfce 4 panels, just pass
`--with-panel=X` to `./configure` when compiling, where X is one of gnome2,
gnome3, mate or xfce4.

If you are compiling from a git clone, you should run `./autogen.sh` instead of
`./configure`.

## FAQ

*   Which Haskell D-Bus package should I use?

    The recommended package is [dbus][5].

*   How to add applets to the GNOME3 panel?

    You need to hold the Alt key when right-clicking the panel.

## Contact

If you have any questions, comments or bug reports, please contact me via GitHub
or drop me a line at  <rohith.reddi9@gmail.com>


[0]: http://uhsure.com/xmonad-log-applet.html
[1]: http://www.haskell.org/haskellwiki/Xmonad/Using_xmonad_in_Gnome
[2]: http://www.haskell.org/haskellwiki/Xmonad/Using_xmonad_in_XFCE
[3]: https://github.com/alexkay/xmonad-log-applet/blob/master/xmonad.hs
[4]: https://xmonad-log-applet.googlecode.com/files/xmonad-log-applet-2.1.0.tar.gz
[5]: http://hackage.haskell.org/package/dbus
[6]: http://versia.com/2011/09/xmonad-log-applet-gnome-xfce/
