Muzei-Bash
==========

  ![Muzei](http://i.imgur.com/vEFoIpw.png)

Port of [Muzei](https://github.com/romannurik/muzei/) to Bash.

Set this script as a(n) (ana)cronjob, and it'll download a new "famous work of art" from WikiPaintings.org everyday and set it as your wallpaper.

Currently supports Linux running in a Gnome-settings-daemon-based environment (Gnome-Shell, Unity, Pantheon, etc.; sets wallpaper via gsettings).  If Gnome-settings-daemon is not running, background is set using [feh](http://feh.finalrewind.org/).  Project is still new, so we don't support blurring or dimming yet (though I don't think those are useful for desktop, unlike smartphones and tablets).

Requirements
------------

* Bash (duh!)
* jq (for parsing Muzei's JSON; can be found in Debian, Ubuntu, Arch AUR, Gentoo, and Fedora repos.  If it's not in your distro's repos, check [here](http://stedolan.github.io/jq/download/).)
* notify-send (for sending "wallpaper changed" notifications)
* feh (only if you aren't running gnome-settings-daemon)
