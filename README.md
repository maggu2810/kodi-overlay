xbmc-overlay
============
A Gentoo overlay which provides modified and unofficial ebuilds
for a XBMC appliance/set-top-box/htpc.

Get it
------
There are two easy ways to get the overlay onto your Gentoo installation:

### 1. Git
1. `mkdir /usr/local/portage`
2. `cd /usr/local/portage`
3. `git clone git://github.com/frace/xbmc-overlay.git`
4. Modify `/etc/make.conf`:

  <pre>
  PORTDIR_OVERLAY="/usr/local/portage/xbmc-overlay/"
  </pre>

### 2. Layman users
If you don't know what `layman` is then please read the [documentation][docs-layman] first.


1. Modify `/etc/layman/layman.cfg`:

  <pre>
  overlays  : http://www.gentoo.org/proj/en/overlays/repositories.xml
              https://raw.github.com/frace/xbmc-overlay/master/repositories.xml
  </pre>

2. Run `layman --list`
3. Run `layman --add xbmc-overlay`

[docs-layman]: http://www.gentoo.org/proj/en/overlays/userguide.xml

Available ebuilds
-----------------

  <pre>
  app-admin/istatd-0.5.7.ebuild
  media-plugins/xbmc-addon-libshairplay-1.0_pre20130416.ebuild
  media-plugins/xbmc-addon-libshairport-1.2.0.20310_pre20130221.ebuild
  media-tv/xbmc-9999.ebuild
  net-fs/afpfs-ng-0.8.1.ebuild
  sys-apps/qingy-1.0.0.ebuild
  </pre>

ToDo
----
- Add an ebuild for a patched («quietboot») version of syslinux
- Add an ebuild for XBMC fbsplash themes in media-gfx/

Links
-----
- [Gentoo dev manual][docs-devmanual]
- [Ebuild writing][docs-devmanual-ebuild]
- [Ebuild file format][docs-devmanual-ebuild-format]

[docs-devmanual]: http://devmanual.gentoo.org/
[docs-devmanual-ebuild]: http://devmanual.gentoo.org/ebuild-writing/
[docs-devmanual-ebuild-format]: http://devmanual.gentoo.org/ebuild-writing/file-format/
