# brightness
Brightness is an extremely simple GNOME dbus daemon wrapper that allows changing screen brightness from the CLI and binding keyboard shortcuts to brightness.

### Operating systems supported
brightness supports, or intends to support, all Linux distributions regardless of kernel version, init system or display protocol assuming the GNOME desktop is installed. It may support BSD or System V distributions of Unix however support is uncertain.

### Installation
1. Git clone this repo: `git clone https://github.com/saltedcoffii/brightness` in a terminal.
2. Install the cloned script into your PATH: `sudo install ./brightness/gnome-brightness /usr/local/bin/gnome-brightness`. I recommend /usr/local/bin, but anywhere in your path will work. If the folder is under the user's home, such as ~/.local/bin/gnome-brightness `sudo` can be omitted.
3. Delete the cloned repo: `rm -rfv ./brightness`

Alternatively, if you're using Ubuntu, Debian, Fedora, CentOS or similar, download a deb or rpm file from the [releases](https://github.com/saltedcoffii/brightness/) page and install with your preferred package manager.

### Usage
To call this program from the CLI while GNOME is running, simply run `gnome-brightness up` or `gnome-brightness down`.

To set a keyboard shortcut, open GNOME's settings, find "Keyboard Shortcuts" on the left hand side, scroll all the way down to the bottom, and click the plus button under "Custom Shortcuts". Add two new shortcuts. One with the name "Brightness up" and command "brightness up", bound to whatever shortcut you like, and the other named "Brightness down" and command "brightness down", bound to whatever shortcut you like.

### Bugs
Please report any new bugs in the issues tab after making sure that the bug hasn't been previously reported. Please provide as much information that you can about your system and why you think it's not working. Pull requests are just as welcome!

### License
This program is licensed under the GNU GPL v3 or later. It is also licensed under the GNU AGPL v3 or later for compatibility purposes.
