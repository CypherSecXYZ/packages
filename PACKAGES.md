# OpenWrt Packages Directory

This document provides a comprehensive directory of packages available in the OpenWrt packages feed, organized by category.

## Table of Contents

- [Admin Tools](#admin-tools)
- [Development Tools](#development-tools)
- [Fonts](#fonts)
- [IPv6 Support](#ipv6-support)
- [Kernel Modules](#kernel-modules)
- [Programming Languages](#programming-languages)
- [Libraries](#libraries)
- [Mail](#mail)
- [Multimedia](#multimedia)
- [Network](#network)
- [Sound](#sound)
- [Utilities](#utilities)

## Admin Tools

The `admin/` directory contains system administration tools and utilities:

| Package | Description |
|---------|-------------|
| htop | Interactive process viewer |
| sudo | Delegate authority to run commands |
| syslog-ng | Powerful syslog daemon |
| zabbix | Enterprise-class monitoring solution |

## Development Tools

The `devel/` directory contains development tools, compilers, and debug utilities:

| Package | Description |
|---------|-------------|
| gcc | GNU Compiler Collection |
| gdb | GNU Debugger |
| pkg-config | Helper tool for compiling applications and libraries |
| scons | Software construction tool |
| trace-cmd | Command line tool for the Linux kernel's ftrace subsystem |

## Fonts

The `fonts/` directory contains font packages for various languages and use cases:

| Package | Description |
|---------|-------------|
| dejavu-fonts-ttf | DejaVu fonts |
| terminus-font | Monospace bitmap font |
| wqy-microhei | Chinese font |

## IPv6 Support

The `ipv6/` directory contains IPv6 related packages and utilities:

| Package | Description |
|---------|-------------|
| 6in4 | IPv6-in-IPv4 tunnel setup |
| 6rd | 6rd tunnel setup |
| 6to4 | 6to4 tunnel setup |

## Kernel Modules

The `kernel/` directory contains kernel modules and extensions:

| Package | Description |
|---------|-------------|
| acx-mac80211 | Driver for TI ACX1xx wireless chipsets |
| hostapd | IEEE 802.11 AP, IEEE 802.1X/WPA/WPA2/EAP Authenticator |
| kmod-wireguard | WireGuard kernel module |

## Programming Languages

The `lang/` directory contains programming languages, interpreters, and language-specific libraries:

| Package | Description |
|---------|-------------|
| golang | Go programming language |
| lua | Lightweight scripting language |
| node | Node.js JavaScript runtime |
| perl | Perl programming language |
| python3 | Python programming language v3.x |
| php8 | PHP scripting language |
| ruby | Ruby programming language |

## Libraries

The `libs/` directory contains general-purpose libraries used by other packages:

| Package | Description |
|---------|-------------|
| libcurl | URL transfers library |
| libjson-c | JSON manipulation library |
| libpcap | Network packet capture library |
| libpng | PNG image library |
| libsqlite3 | SQLite database engine |
| libxml2 | XML parsing library |
| zlib | Compression library |

## Mail

The `mail/` directory contains mail servers, clients, and mail-related utilities:

| Package | Description |
|---------|-------------|
| dovecot | IMAP and POP3 server |
| mutt | Text-based email client |
| postfix | Mail transport agent |

## Multimedia

The `multimedia/` directory contains audio/video applications, codecs, and multimedia tools:

| Package | Description |
|---------|-------------|
| ffmpeg | Audio/video converter |
| gstreamer1 | Multimedia framework |
| minidlna | DLNA/UPnP-AV media server |
| mjpg-streamer | MJPG streamer for webcams |
| youtube-dl | YouTube downloader |

## Network

The `net/` directory contains networking applications, protocols, and utilities:

| Package | Description |
|---------|-------------|
| curl | URL transfers utility |
| mosquitto | MQTT broker |
| nginx | Web server |
| samba4 | SMB/CIFS file, print, and login server |
| tor | Anonymizing overlay network |
| transmission | BitTorrent client |
| wget | Network utility to download files |
| wireguard-tools | WireGuard userspace tools |
| zerotier | Virtual network endpoint |

## Sound

The `sound/` directory contains sound applications, drivers, and audio utilities:

| Package | Description |
|---------|-------------|
| alsa-utils | ALSA sound utilities |
| mpd | Music Player Daemon |
| pulseaudio | Sound system |

## Utilities

The `utils/` directory contains various utilities and tools for system management:

| Package | Description |
|---------|-------------|
| avrdude | AVR microcontroller programmer |
| coreutils | GNU file, shell and text utilities |
| fuse3 | FUSE (Filesystem in Userspace) utilities |
| grep | Pattern matching utilities |
| lm-sensors | Hardware monitoring tools |
| syncthing | Continuous file synchronization program |
| tmux | Terminal multiplexer |
| zstd | Fast real-time compression algorithm |

## Using These Packages

For instructions on how to use these packages in your OpenWrt system, please refer to the [README.md](README.md) file.
