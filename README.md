![CI](https://github.com/bitstower/markets/workflows/CI/badge.svg)
[![Translation](https://hosted.weblate.org/widgets/markets/-/markets/svg-badge.svg)](https://hosted.weblate.org/engage/markets/?utm_source=widget)

![](data/icons/com.bitstower.Markets.svg?raw=true)

# Markets
The Markets application delivers financial data to your fingertips. Track stocks, currencies and cryptocurrencies. Stay on top of the market and never miss an investment opportunity!

## Screenshots

![](preview.png?raw=true)

## Features

* Create your personal portfolio
* Track stocks, currencies, cryptocurrencies, commodities and indexes
* Designed for Phosh (Librem5, PinePhone) and Gnome
* Open any symbol in Yahoo Finance for more details
* Adjust the refresh rate
* Dark Mode

## Installation

> **Librem5 / PinePhone users:** For the best experience, please avoid the Flatpak package and install the app from source. [Flatpak apps don't have access to the patched runtime](https://source.puri.sm/Librem5/Apps_Issues/-/issues/135). Because of that apps are not fully responsive in the Phosh shell. For example dialogs are not maximized.

> **Package mainteners:** We are looking for volunteers to help us make native packages of Markets for Fedora, Debian and other major distributions. It would be great if you could help either by packaging, or by getting the following into the official repositories.

* Flathub: [com.bitstower.Markets](https://flathub.org/apps/details/com.bitstower.Markets)
* Arch (AUR): [bitstower-markets](https://aur.archlinux.org/packages/bitstower-markets/)

## Building from source

### Option 1: with GNOME Builder

1. Open GNOME Builder
1. Click the _Clone Repository_ button
1. Enter `https://github.com/bitstower/markets.git` in the field _Repository URL_
1. Click the _Clone Project_ button
1. Click the _Run_ button to start building application

### Option 2: with Meson

You'll need the following dependencies:

* libsoup
* libgee
* libhandy
* json-glib
* gettext
* glib2
* gtk3
* meson
* vala
* ninja
* git

Clone the repository and change to the project directory

```
git clone https://github.com/bitstower/markets.git
cd markets
```

Run `meson build` to configure the build environment. Change to the build directory and run `ninja` to build

```
meson build --prefix=/usr
cd build
ninja
```

To install, use `ninja install`, then execute with `bitstower-markets`

```
sudo ninja install
bitstower-markets
```

## License

The GNU General Public License, version 3.0 or later
