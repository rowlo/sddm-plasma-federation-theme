# Login manager for Kubuntu 24 LTS SDDM based on SDDM_Plasma by marusyarasskaz.

This modification features a modified version of
[https://forum.elivelinux.org/t/would-like-to-change-login-screen-have-lcars-desktop-gdm-widescreen/3681/4](https://forum.elivelinux.org/t/would-like-to-change-login-screen-have-lcars-desktop-gdm-widescreen/3681/4)
as background using the `LCARS GTJ3.ttf` font of [https://gtjlcars.de/LCARSindex/LCARSFONTS.htm](https://gtjlcars.de/LCARSindex/LCARSFONTS.htm).

That font is licensed as freeware and may not be sold. Therefore, this SDDM theme is not to be charged for and provided free of charge.
With the exception of the font file the rest of the theme is licensed under the GPLv3.

# Credits to the works this theme is based on
- LCARS GTJ3.ttf, by Jens Göttling, Freeware, non-commercial
- SDDM_Plasma served as base, by marusyarasskaz, GPLv3 (This is shipped with Kubuntu 24 LTS only and not available in the KDE Store!)
- background image (adapted), by endarkenment

# Technical details
- location of installed SDDM themes on Kubuntu 24.04: `/usr/share/sddm/themes/`

# Restrictions / Call for Help
That login manager is derived from SDDM_Plasma which is shipped with Kubuntu 24 LTS. That base SDDM project uses Kubuntu specific imports which may not work on other distributions.

I was trying to fix that but had to abort at `BreezeMenuStyle.qml` which uses `QtQuick.Controls.Styles.MenuStyle` from QtQuick Controls version 1. Since Qt 5.12 the QtQuick Controls 1 are deprecated and the styling has been breakingly changed. If you know how to migrate that file to QtQuick Controls 2.12 or newer please feel free to create a [PR on Github](https://github.com/rowlo/sddm-plasma-federation-theme) and I'll update this SDDM login manager.

Until then: This one works only with Kubuntu 24 LTS.
