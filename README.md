# internet-crap

block most of internet crap (fakenews, gambling, malware, adware and porn)

### What is internet-crap
It's a [hosts](hosts) file located in specific directory/folder in your operating system that replaces huge number of fakenews, gambling, malware, adware and porn sites/providers with a non-routable meta-address used to designate an invalid.

### *Source and Inspiration: [StevenBlack's hosts](https://github.com/StevenBlack/hosts)*
### How does it work
When you search something in your web browser it first checks hosts file of your system and then searches for the website in dns server.
So what we are doing is, replacing all those crap websites with [0.0.0.0](https://en.wikipedia.org/wiki/0.0.0.0) before accessing the dns server. And thus, you're unable to access those websites at any cost unless you modify it in the hosts file. Using VPNs are also worthless in this practice.

## Usage
Don't forget to take a backup  of your original host file before replacing it.
### Windows 
locate your hosts file at: `%SystemRoot%\system32\drivers\etc\hosts` and replace it [with the hosts file linked here](hosts).
### Linux
Locate your hosts file at: `/etc/hosts` and replace it [with the hosts file linked here](hosts).
### macOS (until 10.14.x macOS Mojave)
Locate your hosts file at: `/etc/hosts` and replace it [with the hosts file linked here](hosts).
### macOS Catalina
Locate your hosts file at: `/private/etc/hosts` and replace it [with the hosts file linked here](hosts).

### Preview [hosts](https://raw.githubusercontent.com/YogeshLamichhane/internet-crap/main/hosts)
#### Check what's there in hosts file [here](https://raw.githubusercontent.com/YogeshLamichhane/internet-crap/main/hosts). Cause the file is too large to show the preview directly.

### How to add more websites in block list?
	1. Identify the website you want to block in your system. For example: example.xyz
	2. Open your hosts file in your computer and append the following:
	
	0.0.0.0    example.xyz
