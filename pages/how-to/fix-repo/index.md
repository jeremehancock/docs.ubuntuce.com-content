# Fix Repository Issues

Unfortunately, during development of new features for UbuntuCE the UbuntuCE Repository GPG key had to be replaced. This will cause issues when updating software.

The fix is easy. Simply re-run the command below and it should fix the issue.

We have put in some safeguards to prevent this from happening in the future.

---

**Add UbuntuCE Repo Key**


`wget https://job.ubuntuce.com/KEY.gpg && gpg --output ubuntuce.gpg --dearmor KEY.gpg && sudo mv ubuntuce.gpg /usr/share/keyrings/ && rm KEY.gpg`

**Update Packages**

`sudo apt update`

