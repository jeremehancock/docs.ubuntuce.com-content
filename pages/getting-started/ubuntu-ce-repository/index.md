# Repository

UbuntuCE utilizes its [own repository](https://github.com/jeremehancock/repo.ubuntuce.com) for the UbuntuCE specific packages.

### Including:
- [UbuntuCE Welcome](https://github.com/jeremehancock/ubuntu-ce-welcome#readme)
- [UbuntuCE Wallpapers](https://github.com/jeremehancock/ubuntu-ce-wallpapers#readme)
- [DNS Minder](https://github.com/jeremehancock/dnsminder#readme)
- [Host Minder](https://github.com/jeremehancock/hostminder#readme)
- [WorshipExtreme Presenter](https://github.com/jeremehancock/worship-extreme-presenter#readme)

--- 

**Already running Ubuntu? Use the instructions below to setup UbuntuCE.**

---

## Add UbuntuCE Repo and Packages

**Add UbuntuCE Repo Key**

`curl -s --compressed "https://repo.ubuntuce.com/KEY.gpg" | sudo apt-key add -`

**Add UbuntuCE Repo**

`sudo curl -s --compressed -o /etc/apt/sources.list.d/ubuntuce.list "https://repo.ubuntuce.com/ubuntuce.list"`

**Update Packages**

`sudo apt update`

**Install UbuntuCE Packages**

`sudo apt install dnsminder hostminder ubuntu-ce-wallpapers ubuntu-ce-welcome worship-extreme-presenter`

**Setup CleanBrowsing or OpenDNS FamilyShield**

DNS Minder allows you to enable [CleanBrowsing](https://cleanbrowsing.org/) or [OpenDNS FamilyShield](https://www.opendns.com/setupguide/#familyshield).

![DNS Minder](https://raw.githubusercontent.com/jeremehancock/docs.ubuntuce.com-content/main/pages/assets/images/dnsminder-window.png)

---

**UbuntuCE also includes packages outside the UbuntuCE Repo. Use the instructions below to add these packages.**

---

## Add Additional Packages included in UbuntuCE

**Enable Universe/Multiverse Repos**

`sudo add-apt-repository universe`

`sudo add-apt-repository multiverse`

**Add CrossWire PPA**

`sudo add-apt-repository ppa:pkgcrosswire/ppa`

**Update Packages**

`sudo apt update`

**Install Xiphos, BibleTime, Bibledit, Bibledit-Desktop, Sword WEB, Sword KJC, OpenLP**

`sudo apt install xiphos bibletime sword-text-web sword-text-kjv bibledit bibledit-desktop python3-distutils openlp`

