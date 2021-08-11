# Use OpenDNS FamilyShield

UbuntuCE comes pre-configured with web content filtering powered by [CleanBrowsing](https://cleanbrowsing.org/). In our tests [CleanBrowsing](https://cleanbrowsing.org/) provided better protection. However, one issue that we found was the lack of a "block page" to let the user know why they can't load the page.

As an alternative you can use [OpenDNS FamilyShield](https://www.opendns.com/setupguide/#familyshield) instead. It does a good job of blocking most inappropriate content and comes with a nice "block page" as well.

**Open Terminal**

Run `sudo gedit /etc/resolvconf/resolv.conf.d/head`

Edit the `nameserver` entries to match the following

```nameserver 208.67.222.123```

```nameserver 208.67.220.123```

Save the file and close gedit.
	
Run `sudo resolvconf -u` in your terminal.

Done! 

---

If you decide that you would like to go back to [CleanBrowsing](https://cleanbrowsing.org/) follow the steps below.

**Open Terminal**

Run `sudo gedit /etc/resolvconf/resolv.conf.d/head`

Edit the `nameserver` entries to match the following

```nameserver 185.228.168.168```

```nameserver 185.228.169.168```

Save the file and close gedit.
	
Run `sudo resolvconf -u` in your terminal.

Done! 

---

**Note:** *These instructions assume that you haven't made any changes to the network configuration of your UbuntuCE installation.*




