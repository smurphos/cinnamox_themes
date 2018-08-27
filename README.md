Cinnamox Themes
=====

## Introduction

A set of themes for the [Cinnamon](http://developer.linuxmint.com/projects/cinnamon-projects.html) desktop environment.

Each theme includes a Cinnamon desktop theme along with Metacity theme for borders and controls and GTK2, GTK3.18 and GTK 3.20+ themes for applications.

## Credits

Build tools are at [Cinnamox-gtk-theme](https://github.com/smurphos/cinnamox-gtk-theme).

[Cinnamox-gtk-theme](https://github.com/smurphos/cinnamox-gtk-theme) is a fork of [Oomox-gtk-theme](https://github.com/actionless/oomox-gtk-theme).

The Cinnamon themes in both [Cinnamox-gtk-theme](https://github.com/smurphos/cinnamox-gtk-theme) & [Oomox-gtk-theme](https://github.com/actionless/oomox-gtk-theme) are authored by [@smurphos](https://github.com/smurphos).

GTK2, GTK3, GTK3.20 and Metacity themes in both [Cinnamox-gtk-theme](https://github.com/smurphos/cinnamox-gtk-theme) & [Oomox-gtk-theme](https://github.com/actionless/oomox-gtk-theme) are authored by [@Actionless and others](https://github.com/smurphos/cinnamox-gtk-theme/blob/master/CREDITS) with contributions from [@smurphos](https://github.com/smurphos)

Menu in screenshots is the excellent [CinnVIIStarkMenu](https://cinnamon-spices.linuxmint.com/applets/view/281).

Icons in screenshots are from [Vibrancy Colours](http://www.ravefinity.com/p/vibrancy-colors-gtk-icon-theme.html).

## Installation

Install via Cinnamon's Themes module in Cinnamon settings or download from [the release page](https://github.com/smurphos/cinnamox_themes/releases) and unzip into your `~/.themes` directory.

The themes are also hosted on [Cinnamon Spices](https://cinnamon-spices.linuxmint.com/themes) and [openDesktop.org](https://www.opendesktop.org/member/491875).

Once installed select the Cinnamox theme as your Desktop, Controls and Window Borders in the Cinnamon Themes module.

To allow the GTK2, GTK3 and Metacity1 themes to apply to GUI apps running as root run this command in your terminal after installation to create symlinks to user themes in the system theme directory.

`sudo ln -s ~/.themes/* /usr/share/themes/`

## Tweaking

### Cinnamon Theme Transparency

The themes include an interactive bash script that allows end users to adjust the transparency of the Cinnamon Theme. The default is no transparency.

To access the tool open a terminal window (Ctrl-Alt-T) and replacing `$THEME_NAME` with the actual name of the variant installed use the following command to make the script executable and launch it. 

`chmod +x ~/.themes/$THEME_NAME/cinnamon/cinnamox_transparency.sh && ~/.themes/$THEME_NAME/cinnamon/cinnamox_transparency.sh`

If you are not happy with the end result simply run `~/.themes/$THEME_NAME/cinnamon/cinnamox_transparency.sh` again to chose another option including the default.

### GTK2 HIDPI support

If you need HIDPI Support in GTK2 the themes include a HIDPI version of the gtkrc theme file and a helper script to toggle between the regular and HIDPI version.

To run the script open a terminal window (Ctrl-Alt-T) and replacing `$THEME_NAME` with the actual name of the variant installed use the following command to make the script executable and launch it. 

`chmod +x ~/.themes/$THEME_NAME/gtk-2.0/cinnamox_toggle_GTK2_HIDPI.sh && ~/.themes/$THEME_NAME/gtk-2.0/cinnamox_toggle_GTK2_HIDPI.sh`

After the first run you can toggle between the two using `~/.themes/$THEME_NAME/gtk-2.0/cinnamox_toggle_GTK2_HIDPI.sh`

### qt5ct support

If you need support for qt5ct configuration the themes include a premade qt5ct.conf file and a helper script to install it to the correct location `~/.config/qt5ct/colors`

To run the script open a terminal window (Ctrl-Alt-T) and replacing `$THEME_NAME` with the actual name of the variant installed use the following command to make the script executable and launch it.

`chmod +x ~/.themes/$THEME_NAME/qt5ct/cinnamox_enable_qt5ct.sh && ~/.themes/$THEME_NAME/qt5ct/cinnamox_enable_qt5ct.sh`

## Compatibility

Thesw themes are compatible with Cinnamon versions `3.2.x`, `3.4.x`, `3.6.x` & `3.8.x`

The GTK3 themes require GTK `3.18.x` or `3.22.x`

The GTK2 theme requires the package `gtk2-engines-murrine` or `gtk-engine-murrine` to be installed. The former is a default package in Linux Mint.

Tested on Linux Mint `18.2`, `18.3` & `19` 64bit with Cinnamon `3.4.x`, `3.6.x` & `3.8.x`; Also tested ion Manjaro `17.0.6` 64Bit with Cinnamon `3.6.x` & `3.8.x`.

### Firefox fix

If you have problems seeing text on input fields in Firefox with any particular theme this problem can be solved by adding a `~/.mozilla/firefox/********.default/user.js` file to your Firefox default profile including the line `user_pref("widget.content.gtk-theme-override", "Adwaita");` and restarting Firefox.

This forces firefox to use the GTK default Adwaita theme for rendering all website content.

The theme includes a helper script that creates the file with this content in the correct location. To access the tool open a terminal window and use the following command to make the script executable and launch it.

`chmod +x ~/.themes/#THEMENAME/cinnamox_firefox_fix.sh && ~/.themes/#THEMENAME/cinnamon/cinnamox_firefox_fix.sh`

# Make your own theme using Cinnamox / Oomox

The repository at [Cinnamox_theme_master](https://github.com/smurphos/cinnamox_theme_master) includes instructions to utilise the tools provided to make your own unique Cinnamox based theme.

The [Oomox app](https://github.com/actionless/oomox) is a GUI app to design and build themes using the [Oomox-gtk-theme](https://github.com/actionless/oomox-gtk-theme). From [version 1.60+](https://github.com/actionless/oomox/releases/) this app included a Cinnamon theme based on Cinnamox and has an option to export a Cinnamon theme. 

## Changelog & Previous Releases

See [my Github repository](https://github.com/smurphos/cinnamox_themes/releases)

## Screenshots

##### Cinnamox-Aubergine

![Cinnamox-Aubergine](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Aubergine-menu.png "Cinnamox-Aubergine")
![Cinnamox-Aubergine](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Aubergine-calendar.png "Cinnamox-Aubergine")
![Cinnamox-Aubergine](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Aubergine-GTK.png  "Cinnamox-Aubergine")
![Cinnamox-Aubergine](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Aubergine-trans.png  "Cinnamox-Aubergine")

##### Cinnamox-Gold-Spice

![Cinnamox-Gold-Spice](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Gold-Spice-menu.png "Cinnamox-Gold-Spice")
![Cinnamox-Gold-Spice](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Gold-Spice-calendar.png "Cinnamox-Gold-Spice")
![Cinnamox-Gold-Spice](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Gold-Spice-GTK.png  "Cinnamox-Gold-Spice")
![Cinnamox-Gold-Spice](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Gold-Spice-trans.png  "Cinnamox-Gold-Spice")

##### Cinnamox-Heather

![Cinnamox-Heather](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Heather-menu.png "Cinnamox-Heather")
![Cinnamox-Heather](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Heather-calendar.png "Cinnamox-Heather")
![Cinnamox-Heather](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Heather-GTK.png  "Cinnamox-Heather")
![Cinnamox-Heather](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Heather-trans.png  "Cinnamox-Heather")

##### Cinnamox-Kashmir-Blue

![Cinnamox-Kashmir-Blue](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Kashmir-Blue-menu.png "Cinnamox-Kashmir-Blue")
![Cinnamox-Kashmir-Blue](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Kashmir-Blue-calendar.png "Cinnamox-Kashmir-Blue")
![Cinnamox-Kashmir-Blue](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Kashmir-Blue-GTK.png  "Cinnamox-Kashmir-Blue")
![Cinnamox-Kashmir-Blue](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Kashmir-Blue-trans.png  "Cinnamox-Kashmir-Blue")

##### Cinnamox-Rhino

![Cinnamox-Rhino](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Rhino-menu.png "Cinnamox-Rhino")
![Cinnamox-Rhino](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Rhino-calendar.png "Cinnamox-Rhino")
![Cinnamox-Rhino](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Rhino-GTK.png  "Cinnamox-Rhino")
![Cinnamox-Rhino](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Rhino-trans.png  "Cinnamox-Rhino")

##### Cinnamox-Rosso-Cursa

![Cinnamox-Rosso-Cursa](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Rosso-Cursa-menu.png "Cinnamox-Rosso-Cursa")
![Cinnamox-Rosso-Cursa](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Rosso-Cursa-calendar.png "Cinnamox-Rosso-Cursa")
![Cinnamox-Rosso-Cursa](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Rosso-Cursa-GTK.png  "Cinnamox-Rosso-Cursa")
![Cinnamox-Rosso-Cursa](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Rosso-Cursa-trans.png  "Cinnamox-Rosso-Cursa")

##### Cinnamox-Willow-Grove

![Cinnamox-Willow-Grove](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Willow-Grove-menu.png "Cinnamox-Willow-Grove")
![Cinnamox-Willow-Grove](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Willow-Grove-calendar.png "Cinnamox-Willow-Grove")
![Cinnamox-Willow-Grove](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Willow-Grove-GTK.png  "Cinnamox-Willow-Grove")
![Cinnamox-Willow-Grove](https://github.com/smurphos/cinnamox_themes/raw/master/Screenshots/Willow-Grove-trans.png  "Cinnamox-Willow-Grove")

