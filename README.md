# internet-crap

block most of internet crap (fakenews, gambling, malware, adware and porn)

### What is internet-crap
It's a [hosts](hosts) file that is placed somewhere in your computer in a specific folder that replaces all the fakenews, gambling, malware, adware and porn sites/providers with a non-routable meta-address used to designate an invalid.

Inspired and created after watching [StevenBlack's hosts](https://github.com/StevenBlack/hosts).
#### How does it work
huge collection of crap distributors is listed in the hosts and is replaced by [0.0.0.](https://en.wikipedia.org/wiki/0.0.0.0)


## Usage
Don't forget to take a backup  of your original host file before replacing it.
### Windows 
locate your hosts file at: `%SystemRoot%\system32\drivers\etc\hosts` and replace it with [this host file](hosts)
### Linux
Locate your hosts firl at: `/etc/hosts` and replace it with [this host file](hosts)
### macOS (until 10.14.x macOS Mojave)
Locate your hosts firl at: `/etc/hosts` and replace it with [this host file](hosts)
### macOS Catalina
Locate your hosts firl at: `/private/etc/hosts` and replace it with [this host file](hosts)

### How to block your custom websites in youe computer (How to add more websites in block list)
	1. Identify the website you want to block in your system. For example: https://example.xyz
	2. Open your hosts file in your computer and append the following:
	
	0.0.0.0    https://example.xyz
