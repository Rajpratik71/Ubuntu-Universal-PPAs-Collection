# Ubuntu-Universal-PPAs-Collection

This repository contains collection of customized, updated, ported and backported
packages for two last LTS releases and latest pre-LTS release.
Packages for older releases relocated to ppa:eugenesan/archive or deleted.

+-------------------------------------------------------------------------------------+
| Disclaimer:
+-------------------------------------------------------------------------------------+
* Packages in this a nd related PPAs are for personal use only.
  They developed specifically for several custom environments and may not work for you.
* Usage of packages in this PPA, in some forms, might contradict licenses of software
  packaged in this and related PPAs. End users and administrator are responsible for
  runtime licensing and possible legal consequences.
* Some packages provided with their dependencies while some might require additional
  Ubuntu repositories and external PPAs. Below is the list of

+-------------------------------------------------------------------------------------+
| To add this repository, to your Ubuntu installation, invoke:
+-------------------------------------------------------------------------------------+
$ sudo add-apt-repository ppa:eugenesan/ppa

+-------------------------------------------------------------------------------------+
| To access experimental packages before they enter main PPA, invoke:
+-------------------------------------------------------------------------------------+
$ sudo add-apt-repository ppa:eugenesan/boiler

+-------------------------------------------------------------------------------------+
| To access archived/outdated packages, invoke:
+-------------------------------------------------------------------------------------+
$ sudo add-apt-repository ppa:eugenesan/archive

+-------------------------------------------------------------------------------------+
| Packages are maintained for 2 latest LTSs, latest release and upcomming releases:
| Name | Precise | Trusty | Saucy | Utopic | Comments
+-------------------------------------------------------------------------------------+
acroread-fonts-xtd + - - -
aget + - - -
audio-recorder + - - -
autossh + + + -
bcmwl + + + -
bfgminer - + - -
bitcoin - + - -
btsync + + + -
bup + + + -
caffeine + + - - Inhabitant indicator
cardapio - + - -
cdcat + - - -
codelite + + - - Programmer's IDE
ctorrent + + + -
dialog + + - -
dispad + - - -
exfat + + + -
fuse-adbfs + - - -
fusecompress + - - -
gnome-window-applets + + + +
gwoffice + - - -
handbrake + - - -
indicator-sensors + + - -
launchpad-getkeys + - - -
lib7zip + - - -
libapache2-mod-auth-timeout + - - -
libmediainfo + - - -
libmtp + - - -
libvdpau + - - -
libzen + - - -
lsyncd + + - - Resident synchronizer using Rsync
macfanctld - + - -
mc + + + - Midnight Commander
mdadm + - - -
mtpfs + - - -
nuitka + + + - Python to C++ compiler
nxclient + + - -
nxnode + + - -
nxserver + + - -
pianobar + - - -
pica-pica + + - -
rdiff-backup + + + -
reaver + - - -
s3ql + + - -
simple-mtpfs + + - -
skype-call-recorder + - - -
skypetab-ng + + - -

smartgithg + + + - Git+Hg GUI
sparkleshare + + + - Git based Sync client
sslh + - - -
synergy + + + -
tinyxml2 + - - -
truecrypt + + + -
unison + + - -
utouch-geis + - - -
whdd - + + -
wireshark + - - -
wxwidgets2.9 + + - -
xserver-xorg-video-nestedv + - - -
xserver-xorg-video-qxl - + + -
zbackup + + + -

+-------------------------------------------------------------------------------------+
| Next package are kept for historical reasons and no more actively maintained:
+-------------------------------------------------------------------------------------+
nginx (NginX)
php (PHP: Hypertext Preprocessor)
archfs (rdiff-backup as file system)
asterisk
kate (Kate from KDE3 with Kscope)
opennx (OpenNX)
neatx (Google NeatX)
gm-notify (GMail indicator)
googsystray (Google tray notifier)
google-doc-fs (Google Docs/Drive as file system)
transmission (Bittorrent client)
transgui (Remote GUI for transmission)
codeblocks (Programmer's IDE)
efax-gtk (GTK GUI for efax)
audacity (Graphical swiss knife for audio)
audacious (Originally WinAmp clone)
grub2 (Boot Loader)
git (DSC toolkit)
icaterm (Citrix Client)
lexmarkjet (Printer Drivers)
komposer (Mozilla based HTML editor)
meld (Graphical comparator)
moon (Mono IDE)
motion (Motion video detector/recorder)
mydns (*SQL based DNS server)
networkmanager (Networking Manager system)
phc-intel (Tuned for power efficiency Kernel and Tools)
ppa-purge
radiotray
sshguard (SSH Guard daemon, protects from bruteforce attacks)
screen
smartgit (Git GUI replaced by smartgithg)
initramfs-tools
pureftpd
xplanetfx
wxwidgets
ubuntusunrise (Boot Splash Screen)
startupmanager
ttf-fixedsys-excelsior (Free clone of DOS fixed font),
ttf-mscorefonts-installer (Extended MS fonts installer)

+-------------------------------------------------------------------------------------+
| To prevent automatic installation of packages from specific repository, invoke:
+-------------------------------------------------------------------------------------+
$ echo -e "Package: *\n\nPin: release o=LP-PPA-[USER]-[NAME]\nPin-Priority: -1\n\n" | sudo tee -a /etc/apt/preferences
* Replace [USER] and [NAME] with corresponding values (for ex. ajf and trg) or replace whole "LP-PPA-[USER]-[NAME]" string with "Origin" value from appropriate /var/lib/apt/lists/*_Release

+-------------------------------------------------------------------------------------+
| From time to time maintenance of some packages in this repository might be stopped in
| favor of better support by canonical team, official author or a friendly repository.
