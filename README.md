# KDE Plasma Mods

A few mods for the KDE Plasma desktop

## Folder view as a list

Folder view, when placed on the desktop will behave the same as on the panel,
including to show a list of files instead of a grid of icons.

    plasma-desktop-folder-view-list-view.diff


## Change the font of the keyboard layout applet

The font for the keyboard layout applet will be changed to Fira Sans.

This is useful if you use bitmap fonts which the keyboard layout applet
does not support.

    plasma-desktop-keyboard-layout-fira-sans.diff

You need to recompile Plasma after applying this patch.


## Remove icons from the desktop by default

Since some time now, the default for plasma is to show the Desktop folder contents.
This patch reverts to the old Plasma 4.x behaviour which shows an empty desktop
you can manually add the folder view to.

    plasma-desktop-no-folderview-by-default.diff


## Shows the current activity icon on the activity switching applet

By default, the activity switching applet shows a three-dots icon.
If you'd like it to show the current activity icon instead,
apply this patch.

    plasma-desktop-show-activity-manager-current-icon.diff


## Make the volume OSD smaller

Makes the volume (and other) OSD smaller.

    plasma-workspace-small-osd.diff

If the patching fails, you can try copying the following file directly:

    plasma-workspace:lookandfeel:contents:osd:OsdItem.qml
