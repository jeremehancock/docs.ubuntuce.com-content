# Repository

UbuntuCE utilizes its own repository for the UbuntuCE specific packages.

### Including:
- [UbuntuCE Welcome](https://github.com/jeremehancock/ubuntu-ce-welcome#readme)
- [UbuntuCE Wallpapers](https://github.com/jeremehancock/ubuntu-ce-wallpapers#readme)
- [DNS Minder](https://github.com/jeremehancock/dnsminder#readme)
- [Host Minder](https://github.com/jeremehancock/hostminder#readme)
- [UbuntuCE Parental Controls](https://github.com/jeremehancock/ubuntu-ce-parental-controls#readme)
- [Presenter by WorshipTools](https://github.com/jeremehancock/presenter-by-worship-tools#readme)
- [FreeShow](https://freeshow.app)

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

`sudo apt install dnsminder hostminder ubuntu-ce-parental-controls ubuntu-ce-wallpapers ubuntu-ce-welcome presenter-by-worship-tools freeshow`

**Setup Web Content Filtering**

DNS Minder allows you to enable [CleanBrowsing](https://cleanbrowsing.org/), [OpenDNS FamilyShield](https://www.opendns.com/setupguide/#familyshield) , [1.1.1.1 for Families](https://blog.cloudflare.com/introducing-1-1-1-1-for-families/), or [AdGuard Family DNS](https://adguard-dns.io/en/public-dns.html).

![DNS Minder](https://raw.githubusercontent.com/jeremehancock/docs.ubuntuce.com-content/main/pages/assets/images/dnsminder-job.png)

**Configure UbuntuCE Plymouth Theme**

`sudo apt install git -y && git clone https://github.com/jeremehancock/ubuntu-ce-plymouth-theme.git && cd ubuntu-ce-plymouth-theme && sudo cp -R ubuntuce /usr/share/plymouth/themes/ && sudo update-alternatives --install "/usr/share/plymouth/themes/default.plymouth" "default.plymouth" "/usr/share/plymouth/themes/ubuntuce/ubuntuce.plymouth" 160 && sudo update-alternatives --auto default.plymouth && sudo update-alternatives --config default.plymouth && sudo update-initramfs -uk all && cd .. && rm -rf ubuntu-ce-plymouth-theme`

**Configure UbuntuCE Login Branding**

`git clone https://github.com/jeremehancock/ubuntu-ce-logos.git && sudo cp ubuntu-ce-logos/usr/share/plymouth/ubuntu-logo.png /usr/share/plymouth/ubuntuce-logo.png && sudo printf "[org.gnome.login-screen]\nlogo='/usr/share/plymouth/ubuntuce-logo.png'" | sudo tee /usr/share/glib-2.0/schemas/90_ubuntu-settings.gschema.override && rm -rf ubuntu-ce-logos && sudo glib-compile-schemas /usr/share/glib-2.0/schemas/`

*Note: You will need to reboot for Plymouth Theme and UbuntuCE Login Branding to take effect*

---

**UbuntuCE also includes packages outside the UbuntuCE Repo. Use the instructions below to add these packages.**

---

## Add Additional Packages included in UbuntuCE

**Enable Universe/Multiverse Repos**

`sudo add-apt-repository universe && sudo add-apt-repository multiverse`

**Install Xiphos, BibleTime, Bibledit, Bible-KJV, Sword WEB, Sword KJC, OpenLP, and Timekpr-nExT**

`sudo apt install xiphos bibletime sword-text-web sword-text-kjv bibledit python3-distutils default-jre libreoffice-java-common openlp bible-kjv timekpr-next`

**Install Flatpak**

`sudo apt install flatpak && sudo flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo`

**Install Bolls Bible, Floodlight Presenter, and Son of Man**

`sudo flatpak install flathub life.bolls.bolls io.gitlab.floodlight.Presenter org.hlwd.sonofman`