# Changelog

Versioning uses a combination of the Ubuntu ISO base that is used to build the release and the date of the build followed by a number. The trailing number is used if there is more than one build on the same day.

## [22.04.0-2022.05.24.0] - 2022-05-24
### <span style="color: black;">Changed</span>
- Updated all UbuntuCE apps to the latest versions

## [22.04.0-2022.05.22.0] - 2022-05-22
### <span style="color: black;">Changed</span>
- Updated all UbuntuCE apps to the latest versions
- Updated neofetch config to include Daily Bible verse
- Removed OpenLP due to issues running on latest Ubuntu LTS. Plan to add it into the new UbuntuCE Software Center once bug is resolved.
- Changed which apps are pre-installed since the new UbuntuCE Software Center will allow easy installations. This will trim the ISO size quite a bit.

### <span style="color: black;">Added</span>
- Added [UbuntuCE Software Center](https://github.com/jeremehancock/ubuntu-ce-software-center#readme)
- Added [UbuntuCE Branding](https://github.com/jeremehancock/ubuntu-ce-branding#readme)
- Added the Catholic Public Domain Version (CPDV)

## [22.04.0-2022.05.12.0] - 2022-05-12
### <span style="color: black;">Changed</span>
- Updated all UbuntuCE apps to the latest versions
- Fixed dark mode wallpaper bug

### <span style="color: black;">Added</span>
- Added [UbuntuCE Parental Controls](https://github.com/jeremehancock/ubuntu-ce-parental-controls#readme)
- Added [Timekpr-nExT](https://mjasnik.gitlab.io/timekpr-next/)
- Added [FreeShow](https://freeshow.app)
- Added customized UbuntuCE installer (English Only)
- Added UbuntuCE branding to the Settings
- Added [UbuntuCE Plymouth Theme](https://github.com/jeremehancock/ubuntu-ce-plymouth-theme) as default
- Added UbuntuCE branding to the login screen
- Added neofetch
- Added `.bash_aliases` file to launch neofetch when terminal is launched

## [22.04.0-2022.04.26.0] - 2022-04-26
### <span style="color: black;">Changed</span>
- Initial Ubuntu 22.04 Release
- Updated Presenter by WorshipTools to pull AppImage down on first launch
- Updated UbuntuCE Welcome app to include Software tab

### <span style="color: black;">Added</span>
- Added Son of Man app
- Added Floodlight Presenter app
- Added Bolls Bible app
- Added AdGuard Family DNS to DNS Minder

## [20.04.4-2022.03.24.0] - 2022-03-24
### <span style="color: black;">Changed</span>
- Updated DNS Minder to latest version
- Updated using the latest Ubuntu LTS base

## [20.04.3-2021.08.24.0] - 2021-08-24
### <span style="color: black;">Changed</span>
- Host Minder now includes an Allow List
- Updated UbuntuCE Welcome with tabbed layout
- Updated using the latest Ubuntu LTS base

### <span style="color: black;">Added</span>
- Added DNS Minder
- Added Configure DNS Minder to UbuntuCE Welcome
- Added options to change wallpaper and them in UbuntuCE Welcome
- Added DNS Minder to favorites

## [20.04.2-2021.08.16.0] - 2021-08-16
### <span style="color: black;">Changed</span>
- Updated to include the latest version of Host Minder
- Host Minder now has a default weekly auto updater

## [20.04.2-2021.08.10.0] - 2021-08-10
### <span style="color: black;">Changed</span>
- Updated UbuntuCE Welcome with UbuntuCE Docs button and Patreon button

## [20.04.2-2021.07.30.0] - 2021-07-30
### <span style="color: black;">Changed</span>
- Switched from [OpenDNS FamilyShield](https://www.opendns.com/setupguide/#familyshield) to [CleanBrowsing](https://cleanbrowsing.org/)
- Updated UbuntuCE Welcome to reflect changes in DNS configuration
- Updated Worship Extreme Presenter with new updater

## [20.04.2-2021.07.29.0] - 2021-07-29
### <span style="color: black;">Added</span>
- Universe Repos
- Multverse Repos
- resolvconf
- vim
- curl
- VLC
- UbuntuCE Repo
- UbuntuCE Welcome
- UbuntuCE Wallpapers
- Host Minder
- WorshipExtreme Presenter
- CrossWire PPA
- Xiphos
- Sword Text WEB
- Sword Text KJV
- BibleEdit
- BibleEdit Desktop
- OpenLP
- BibleTime
- Configured Favorites to the following
	+ UbuntuCE Welcome
	+ FireFox
	+ Host Minder
	+ BibleTime
	+ Xiphos
	+ OpenLP
	+ WorshipExtreme Presenter
- Set UbuntuCE Welcome to launch on startup
- Configured Default wallpaper to `/usr/share/backgrounds/ubuntu-ce-1.jpg`
- Configured [OpenDNS FamilyShield](https://www.opendns.com/setupguide/#familyshield) via resolvconf