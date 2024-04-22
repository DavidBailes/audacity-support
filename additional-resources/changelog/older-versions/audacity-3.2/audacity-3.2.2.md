# Audacity 3.2.2

**Audacity 3.2.2 was released on 06 Dec 2022**

This is a patch release for Audacity 3.2. It enables use of VST2 as realtime effects and fixes some bugs.

## Changes and improvements since previous version

* [#2850](https://github.com/audacity/audacity/issues/2850) VST2 effects are now realtime capable. \
  Additional plugins have been added to [plugins.audacityteam.org](https://app.gitbook.com/o/-MhmG2mhIIHTtQPuHV\_k/s/klCVENFte0GRy5IqVz0W/)
* [#3696](https://github.com/audacity/audacity/pull/3696) Improved accessibility of the meters
* [#3769](https://github.com/audacity/audacity/issues/3769) Fixed a crash when editing some macro parameters
* [#3792](https://github.com/audacity/audacity/issues/3792) Fixed some play commands getting stuck in play mode
* [#3670](https://github.com/audacity/audacity/issues/3670) Audacity no longer quietly discards changes in realtime effects but instead asks if you want to save before quitting
* [#3838](https://github.com/audacity/audacity/issues/3838) Plugin scanning now lets you skip individual plugins if scanning gets stuck on them
* [#3980](https://github.com/audacity/audacity/pull/3980) Plugin scanning no longer produces "Audacity crashed" windows when a plugin fails validation, and no longer shows the plugins in the macOS dock during validation
* [#3883](https://github.com/audacity/audacity/issues/3883) Fixed an issue with labels losing focus on macOS Ventura
* Fixed various plugin-specific issues

A full list of changes can be found [on Github](https://github.com/audacity/audacity/milestone/13?closed=1).

## Supported platforms

**Windows**

* Audacity 3.2 supports Windows 10 & 11
  * Windows Vista, 7 and 8.1 should still work, but are no longer tested.
  * Downloads for older versions are available on the [Legacy Windows](https://www.audacityteam.org/download/legacy-windows/) page on the Audacity Website.

**macOS / Mac OS X**

* Audacity 3.2 supports OS X 10.9 and later, and macOS.
  * There are legacy versions for older OS X at [http://audacityteam.org/download/legacy-mac/](http://audacityteam.org/download/legacy-mac/).

**Linux**

* In addition to the traditional update path via package managers, Audacity 3.0.3 and onwards are distributed as an AppImage. The AppImage gets updated at the same time as the Windows and macOS versions, so if you collaborate with users on those platforms, you may want to use the AppImage over your distribution's package manager.
* Linux support is tested on Ubuntu 20.04.
  * Other Linux distributions should work, but aren't tested by the Audacity team.
