# Firewall for Whonix-Gateway and Whonix-Workstation #

iptables rules script and firewall configuration file for Whonix-Gateway and
Whonix-Workstation.

Whonix-Gateway Firewall Features:
- transparent proxying
- stream isolation
- reject invalid packages
- fail closed mechanism
- optional VPN-Firewall
- optional isolating proxy
- optional incoming flash proxy
- optional Tor relay

Do not remove, unless you no longer wish to use Whonix.
## How to install `whonix-firewall` using apt-get ##

1\. Download Whonix's Signing Key.

```
wget https://www.whonix.org/patrick.asc
```

Users can [check Whonix Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key) for better security.

2\. Add Whonix's signing key.

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/derivative.gpg add ~/patrick.asc
```

3\. Add Whonix's APT repository.

```
echo "deb https://deb.whonix.org buster main contrib non-free" | sudo tee /etc/apt/sources.list.d/derivative.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `whonix-firewall`.

```
sudo apt-get install whonix-firewall
```

## How to Build deb Package from Source Code ##

Can be build using standard Debian package build tools such as:

```
dpkg-buildpackage -b
```

See instructions. (Replace `generic-package` with the actual name of this package `whonix-firewall`.)

* **A)** [easy](https://www.whonix.org/wiki/Dev/Build_Documentation/generic-package/easy), _OR_
* **B)** [including verifying software signatures](https://www.whonix.org/wiki/Dev/Build_Documentation/generic-package)

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Donate ##

`whonix-firewall` requires [donations](https://www.whonix.org/wiki/Donate) to stay alive!
