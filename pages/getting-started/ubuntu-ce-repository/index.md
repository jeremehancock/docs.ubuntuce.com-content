# UbuntuCE Software Center

UbuntuCE utilizes its own repository for the UbuntuCE specific packages.

### Including:
- [UbuntuCE Greeter](https://github.com/jeremehancock/ubuntu-ce-welcome#readme)
- [UbuntuCE Software Center](https://github.com/jeremehancock/ubuntu-ce-software-center#readme)
- [UbuntuCE Branding](https://github.com/jeremehancock/ubuntu-ce-branding#readme)
- [UbuntuCE Wallpapers](https://github.com/jeremehancock/ubuntu-ce-wallpapers#readme)
- [DNS Minder](https://github.com/jeremehancock/dnsminder#readme)
- [Host Minder](https://github.com/jeremehancock/hostminder#readme)
- [UbuntuCE Parental Controls](https://github.com/jeremehancock/ubuntu-ce-parental-controls#readme)
- [Presenter by WorshipTools](https://github.com/jeremehancock/presenter-by-worship-tools#readme)
- [FreeShow](https://freeshow.app)


--- 

**Already running Ubuntu 22.04? Use the instructions below to set up UbuntuCE.**

**Note:** *UbuntuCE only supports the latest LTS.* 

*So you will need to be running Ubuntu 22.04 in order to use the UbuntuCE Repo.*

---

## Add UbuntuCE Repo & UbuntuCE Software Center

**Add UbuntuCE Repo Key**

`wget https://job.ubuntuce.com/KEY.gpg && gpg --output ubuntuce.gpg --dearmor KEY.gpg && sudo mv ubuntuce.gpg /usr/share/keyrings/ && rm KEY.gpg`

**Add UbuntuCE Repo**

`sudo apt install curl -y && sudo curl -s --compressed -o /etc/apt/sources.list.d/ubuntuce-jammy.list "https://job.ubuntuce.com/ubuntuce-jammy.list"`

**Update Packages**

`sudo apt update`

**Install UbuntuCE Software Center**

`sudo apt install ubuntu-ce-software-center -y`

The UbuntuCE Software Center will allow you to easily set up your system with the applications, and branding that comes with UbuntuCE.

![UbuntuCE Software Center](https://raw.githubusercontent.com/jeremehancock/docs.ubuntuce.com-content/main/pages/assets/images/ubuntu-ce-software-center-bible-study.png)
