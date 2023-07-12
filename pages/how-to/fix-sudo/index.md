# Fix sudo issues

If you see the following error in your terminal it could be related to a previous bug in the Host Minder app.

`sudo: unable to resolve host _hostname_: Name or service not known`

---

**How to fix:**

Disable Host Minder if it is currently enabled. 

Be sure your packages are updated by running the following command.

`sudo apt update && sudo apt upgrade`

Run the following command to ensure that your machine's `hostname` is listed in the `/etc/hosts` file.

`sed -i "/^127.0.0.1\ localhost$/ s/$/\ $(hostname)/" /etc/hosts`

Now you can re-enable Host Minder and choose the preferred Protection Level.



