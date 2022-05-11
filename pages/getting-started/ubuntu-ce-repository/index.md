# Repository

UbuntuCE utilizes its own repository for the UbuntuCE specific packages.

### Including:
- [UbuntuCE Welcome](https://github.com/jeremehancock/ubuntu-ce-welcome#readme)
- [UbuntuCE Wallpapers](https://github.com/jeremehancock/ubuntu-ce-wallpapers#readme)
- [DNS Minder](https://github.com/jeremehancock/dnsminder#readme)
- [Host Minder](https://github.com/jeremehancock/hostminder#readme)
- [Presenter by WorshipTools](https://github.com/jeremehancock/presenter-by-worship-tools#readme)

--- 

**Already running Ubuntu 22.04? Use the instructions below to setup UbuntuCE.**

**Note:** *UbuntuCE only supports the latest LTS.* 

*So you will need to be running Ubuntu 22.04 in order to use the UbuntuCE Repo.*

---

## Add UbuntuCE Repo and Packages

**Add UbuntuCE Repo Key**

`wget https://job.ubuntuce.com/KEY.gpg && gpg --output ubuntuce.gpg --dearmor KEY.gpg && sudo mv ubuntuce.gpg /usr/share/keyrings/ && rm KEY.gpg`

**Add UbuntuCE Repo**

`sudo apt install curl -y && sudo curl -s --compressed -o /etc/apt/sources.list.d/ubuntuce-jammy.list "https://job.ubuntuce.com/ubuntuce-jammy.list"`

**Update Packages**

`sudo apt update`

**Install UbuntuCE Packages**

`sudo apt install dnsminder hostminder ubuntu-ce-wallpapers ubuntu-ce-welcome presenter-by-worship-tools`

**Setup Web Content Filtering**

DNS Minder allows you to enable [CleanBrowsing](https://cleanbrowsing.org/), [OpenDNS FamilyShield](https://www.opendns.com/setupguide/#familyshield) , [1.1.1.1 for Families](https://blog.cloudflare.com/introducing-1-1-1-1-for-families/), or [AdGuard Family DNS](https://adguard-dns.io/en/public-dns.html).

![DNS Minder](https://raw.githubusercontent.com/jeremehancock/docs.ubuntuce.com-content/main/pages/assets/images/dnsminder-job.png)

---

**UbuntuCE also includes packages outside the UbuntuCE Repo. Use the instructions below to add these packages.**

---

## Add Additional Packages included in UbuntuCE

**Enable Universe/Multiverse Repos**

`sudo add-apt-repository universe && sudo add-apt-repository multiverse`

**Install Xiphos, BibleTime, Bibledit, Bible-KJV, Sword WEB, Sword KJC, and OpenLP**

`sudo apt install xiphos bibletime sword-text-web sword-text-kjv bibledit python3-distutils default-jre libreoffice-java-common openlp bible-kjv`

**Install Flatpak**

`sudo apt install flatpak && sudo flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo`

**Install Bolls Bible, Floodlight Presenter, and Son of Man**

`sudo flatpak install flathub life.bolls.bolls io.gitlab.floodlight.Presenter org.hlwd.sonofman`