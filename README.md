# unofficial-archrootfs

<p align="left">
  <img src="https://github.com/Zhoneym/unofficial-archrootfs/assets/140673973/3147ae73-4ca8-403d-8942-f1b0d4724f7d" width="512"/>
</p>


This is an unofficial packaging that complies with the OCI standard rootfs and is also applicable to Microsoft WSL2. Originally intended to temporarily replace the construction of the official Docker image in the event of issues with the official Gitlab-CI build，but it is still a relatively ideal choice

 [![Build Arch Linux rootfs](https://github.com/Zhoneym/unofficial-archrootfs/actions/workflows/build.yml/badge.svg)](https://github.com/Zhoneym/unofficial-archrootfs/actions/workflows/build.yml)

Arch Linux, a lightweight and flexible Linux® distribution that tries to Keep It Simple.

Compared to the official Docker image repository, this repository has the following advantages:


 - Faster update frequency
 - A simpler and more transparent packaging method
 - High degree of freedom and customizability

We offer three options:

 - base: Minimal package set to define a basic Arch Linux installation

```bash
docker pull zhoneym/unofficial-archrootfs-base:latest
```

Contains the following software packages:

| Package | Repository |
|-|-|  
| acl | core |
| archlinux-keyring | core |
| argon2 | core |
| attr | core |  
| audit | core |
| bash | core |
| brotli | core |
| bzip2 | core |
| ca-certificates | core |
| ca-certificates-mozilla | core |
| ca-certificates-utils | core |
| coreutils | core |
| cryptsetup | core |
| curl | core |
| dbus | core |
| device-mapper | core |
| e2fsprogs | core |
| expat | core |
| file | core |
| filesystem | core |
| findutils | core |
| gawk | core |
| gcc-libs | core |
| gdbm | core |  
| gettext | core |
| glib2 | core |
| glibc | core |
| gmp | core |
| gnupg | core |
| gnutls | core |
| gpgme | core |
| grep | core |
| gzip | core |
| hwdata | core |
| iana-etc | core |
| icu | core |
| iproute2 | core | 
| iptables | core |
| iputils | core |
| json-c | core |
| kbd | core |
| keyutils | core |
| kmod | core |
| krb5 | core |
| less | core |
| libarchive | core |
| libassuan | core |
| libbpf | core |
| libcap | core |
| libcap-ng | core |  
| libelf | core |
| libevent | core |
| libffi | core |
| libgcrypt | core |
| libgpg-error | core |
| libidn2 | core |
| libksba | core |
| libldap | core |
| libmnl | core |
| libnetfilter_conntrack | core |
| libnfnetlink | core |
| libnftnl | core |
| libnghttp2 | core |
| libnl | core |
| libp11-kit | core |
| libpcap | core |
| libpsl | core |
| libsasl | core |
| libseccomp | core |
| libsecret | core |
| libssh2 | core |
| libsysprof-capture | extra |
| libtasn1 | core |
| libtirpc | core |  
| libunistring | core |
| libutempter | extra |  
| libverto | core |
| libxcrypt | core |
| libxml2 | core |
| licenses | core |
| linux-api-headers | core |
| lz4 | core |
| mpfr | core |
| ncurses | core |
| nettle | core |
| npth | core |
| openssl | core |
| p11-kit | core |
| pacman | core |
| pacman-mirrorlist | core |
| pam | core |
| pambase | core |
| pciutils | core |
| pcre2 | core |
| pinentry | core |
| popt | core |
| procps-ng | core |
| psmisc | core |
| readline | core |
| sed | core |
| shadow | core |
| sqlite | core |  
| systemd | core |
| systemd-libs | core |
| systemd-sysvcompat | core |
| tar | core |
| tpm2-tss | core |
| tzdata | core |
| util-linux | core |
| util-linux-libs | core |
| xz | core |
| zlib | core |
| zstd | core |
| base | core |

 - base-devel: Minimum package set to define a basic Arch Linux installation and basic tools to build Arch Linux packages

```bash
docker pull zhoneym/unofficial-archrootfs-base-devel:latest
```

 - workstations: Contains commonly used compiler tools and common system management tools (this option is very suitable for working with Microsoft WSL2)

```bash
docker pull zhoneym/unofficial-archrootfs-workstations:latest
```

Microsoft WSL2 users please download and manually import from the following link:

https://github.com/Zhoneym/unofficial-archrootfs/releases


Arch Linux official Docker image gitlab repository: https://gitlab.archlinux.org/archlinux/archlinux-docker

OCI-Compatible images for Arch Linux official:

https://hub.docker.com/_/archlinux

https://hub.docker.com/r/archlinux/archlinux/

https://quay.io/repository/archlinux/archlinux

https://github.com/archlinux/archlinux-docker/pkgs/container/archlinux
