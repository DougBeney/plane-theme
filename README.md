<p align="center">
<img src="assets/logo.svg" />
</p>


# PLANE THEME

- 	A beautiful theme for Gnome Linux, more information in [Plane project](https://github.com/wfpaisa/plane)

<p align="center">
<img src="assets/screenshots/screenshot-01.png" />
<br>
<img src="assets/screenshots/screenshot-02.png" />
<br>
<img src="assets/screenshots/screenshot-03.png" />
<br>
<img src="assets/screenshots/screenshot-04.png" />
<br>
<img src="assets/screenshots/screenshot-05.png" />
<br>
<img src="assets/screenshots/screenshot-06.jpeg" />
</p>

## Build

NODE: v8.12.0

NPM:  v6.4.1

```bash 

# Install node modules
$ npm i

# Build
$ gulp

# Copy white variant
$ sudo cp -a ./build/Plane /usr/share/themes/Plane

# Copy dark variant
$ sudo cp -a ./build/Plane-dark /usr/share/themes/Plane-dark

# Active white theme
$ gsettings set  org.gnome.desktop.interface gtk-theme Plane && gsettings set org.gnome.shell.extensions.user-theme name Plane

# Active dark theme
$ gsettings set  org.gnome.desktop.interface gtk-theme Plane-dark && gsettings set org.gnome.shell.extensions.user-theme name Plane-dark

```


## Build with Autoreload

```bash 

# Build and make symbolic link to themes
$ npm i
$ gulp
$ CURR_DIR=$(pwd)
$ sudo ln -s ${CURR_DIR}/build/Plane /usr/share/themes/Plane
$ sudo ln -s ${CURR_DIR}/build/Plane-dark /usr/share/themes/Plane-dark

# Autoreload Plane
$ gulp watch

# Autoreload Plane-dark
$ gulp watch -D

```


## Update

Upstream themes are downloaded and changes monitored.

- Gtk: `/upstream/gtk-3.0` -> https://github.com/GNOME/gtk/tree/master/gtk/theme/Adwaita
- Gnome-shell: `upstream/gnome-shell` -> https://github.com/GNOME/gnome-shell/tree/master/data/theme


## GDM Theme
You can change the GDM (lock/login screen) theme by replacing the default GNOME Shell theme.
See the wiki for details: https://github.com/wfpaisa/plane-theme/wiki/GDM-Theme

## Thanks to

- Arc Theme
- Adwaita Theme

And all those designs that served as inspiration

