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

Contains the following software packages:

| Package | Repository |
|-|-|
| acl | core |
| archlinux-keyring | core |  
| argon2 | core |
| attr | core |
| audit | core |
| autoconf | core |
| automake | core |
| bash | core |
| binutils | core |
| bison | core |
| brotli | core |
| bzip2 | core |
| ca-certificates | core |
| ca-certificates-mozilla | core |
| ca-certificates-utils | core |
| coreutils | core |
| cryptsetup | core |
| curl | core |
| db | core |
| db5.3 | core |
| dbus | core |
| debugedit | core |
| device-mapper | core |
| diffutils | core |
| e2fsprogs | core |
| expat | core |
| fakeroot | core |
| file | core |
| filesystem | core |
| findutils | core |  
| flex | core |
| gawk | core |
| gc | core |
| gcc | core |
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
| groff | core |
| guile | core |
| gzip | core |
| hwdata | core |
| iana-etc | core |
| icu | core |
| iproute2 | core |
| iptables | core |
| iputils | core |
| jansson | core |
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
| libisl | core |
| libksba | core |
| libldap | core |
| libmnl | core |
| libmpc | core |
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
| libtool | core |
| libunistring | core |
| libutempter | extra |
| libverto | core |
| libxcrypt | core |
| libxml2 | core |
| licenses | core |
| linux-api-headers | core |
| lz4 | core |  
| m4 | core |
| make | core |
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
| patch | core |
| pciutils | core |
| pcre2 | core |
| perl | core |
| pinentry | core |
| pkgconf | core |
| popt | core |
| procps-ng | core |
| psmisc | core |
| readline | core |
| sed | core |
| shadow | core |
| sqlite | core |
| sudo | core |
| systemd | core |
| systemd-libs | core |
| systemd-sysvcompat | core |
| tar | core |
| texinfo | core |
| tpm2-tss | core |
| tzdata | core |
| util-linux | core |
| util-linux-libs | core |
| which | core |
| xz | core |
| zlib | core |
| zstd | core |
| base | core |
| base-devel | core |

 - workstations: Contains commonly used compiler tools and common system management tools (this option is very suitable for working with Microsoft WSL2)

```bash
docker pull zhoneym/unofficial-archrootfs-workstations:latest
```

Contains the following software packages:

| Package | Repository |
|-|-|
| acl | core |
| archlinux-keyring | core |
| argon2 | core |
| attr | core |
| audit | core |
| autoconf | core |
| automake | core |
| bash | core |
| binutils | core |
| bison | core |
| bluez-libs | extra |
| boost-libs | extra |  
| brotli | core |
| bzip2 | core |
| c-ares | extra |
| ca-certificates | core |
| ca-certificates-mozilla | core |
| ca-certificates-utils | core |
| compiler-rt | extra |
| coreutils | core |  
| cppdap | extra |
| cryptsetup | core |
| curl | core |
| db | core |
| db5.3 | core |
| dbus | core |
| debugedit | core |
| device-mapper | core |
| diffutils | core |
| duktape | extra |
| e2fsprogs | core |
| expat | core |
| fakeroot | core |
| file | core |
| filesystem | core |
| findutils | core |
| flex | core |
| gawk | core |  
| gc | core |
| gcc | core |
| gcc-libs | core |
| gdbm | core |
| gettext | core |
| glib2 | core |
| glibc | core |
| gmp | core |
| gnupg | core |
| gnutls | core |
| gpgme | core |
| gpm | core |
| grep | core |
| groff | core |  
| guile | core |
| gzip | core |
| hicolor-icon-theme | extra |
| hwdata | core |
| iana-etc | core |
| icu | core |
| iproute2 | core |
| iptables | core |
| iputils | core |
| jansson | core |
| json-c | core |
| jsoncpp | extra |
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
| libdaemon | extra |
| libedit | core |
| libelf | core |
| libevent | core |
| libffi | core |  
| libgcrypt | core |  
| libgpg-error | core |
| libidn2 | core |
| libisl | core |
| libksba | core |
| libldap | core |
| libmm-glib | extra |
| libmnl | core |
| libmpc | core |
| libndp | extra |
| libnetfilter_conntrack | core |
| libnewt | extra |
| libnfnetlink | core |  
| libnftnl | core |
| libnghttp2 | core |
| libnl | core |  
| libnm | extra |
| libnsl | core |
| libp11-kit | core |
| libpcap | core |
| libpgm | extra |
| libpsl | core |
| libsasl | core |
| libseccomp | core |
| libsecret | core |  
| libsodium | extra |
| libssh2 | core |
| libsysprof-capture | extra |  
| libtasn1 | core |
| libteam | extra |
| libtirpc | core |
| libtool | core |
| libunistring | core |
| libutempter | extra |
| libuv | extra |
| libverto | core |
| libxcrypt | core |  
| libxml2 | core |
| libyaml | extra |
| licenses | core |
| linux-api-headers | core |
| llvm-libs | extra |
| m4 | core |
| make | core |
| mobile-broadband-provider-info | extra |  
| mpfr | core |
| ncurses | core |
| nettle | core |  
| npth | core |
| nspr | core |
| nss | core |
| p11-kit | core |
| pacman | core |
| pacman-mirrorlist | core |
| pam | core |  
| pambase | core |
| patch | core |
| pciutils | core |
| pcre | core |
| pcre2 | core |
| pcsclite | extra |
| perl | core |
| perl-error | extra |
| perl-mailtools | extra |  
| perl-timedate | extra |
| pinentry | core |
| pkgconf | core |
| polkit | extra |
| popt | core |
| procps-ng | core |  
| psmisc | core |
| python-six | extra |
| readline | core |
| rhash | extra |
| ruby-abbrev | extra |
| ruby-base64 | extra |  
| ruby-benchmark | extra |
| ruby-bigdecimal | extra |  
| ruby-bundledgems | extra |
| ruby-bundler | extra |
| ruby-cgi | extra |
| ruby-csv | extra |
| ruby-date | extra |  
| ruby-delegate | extra |
| ruby-did_you_mean | extra |
| ruby-digest | extra |
| ruby-drb | extra |
| ruby-english | extra |
| ruby-erb | extra |
| ruby-etc | extra |
| ruby-fcntl | extra |  
| ruby-fiddle | extra |
| ruby-fileutils | extra |
| ruby-find | extra |
| ruby-forwardable | extra |
| ruby-getoptlong | extra |
| ruby-io-console | extra |
| ruby-io-nonblock | extra |
| ruby-io-wait | extra |
| ruby-ipaddr | extra |  
| ruby-irb | extra |
| ruby-json | extra |
| ruby-logger | extra |
| ruby-minitest | extra |
| ruby-mutex_m | extra |
| ruby-net-http | extra |
| ruby-open-uri | extra |
| ruby-power_assert | extra |  
| ruby-psych | extra |
| ruby-racc | extra |
| ruby-rake | extra |
| ruby-rdoc | extra |
| ruby-reline | extra |
| ruby-rexml | extra |
| ruby-ruby2_keywords | extra |
| ruby-stdlib | extra |  
| ruby-stringio | extra |
| ruby-test-unit | extra |
| ruby-time | extra |
| ruby-tmpdir | extra |
| ruby-uri | extra |
| rubygems | extra |
| sed | core |
| shadow | core |  
| slang | extra |
| sqlite | core |
| systemd | core |
| systemd-libs | core |
| systemd-sysvcompat | core |
| tar | core |
| texinfo | core |
| tpm2-tss | core |  
| tzdata | core |
| util-linux | core |
| util-linux-libs | core |
| which | core |
| wpa_supplicant | core |
| xz | core |
| zeromq | extra |
| base | core |
| base-devel | core |  
| boost | extra |
| clang | extra |
| cmake | extra |
| fmt | extra |
| git | extra |
| glslang | extra |
| go | extra |  
| lldb | extra |
| llvm | extra |
| lz4 | core |
| neofetch | extra |
| net-tools | core |
| networkmanager | extra |
| ninja | extra |
| nodejs | extra |
| openssl | core |  
| pacman-contrib | extra |
| python | core |
| ruby | extra |
| rust | extra |
| sudo | core |
| zlib | core |
| zstd | core |
Microsoft WSL2 users please download and manually import from the following link:

https://github.com/Zhoneym/unofficial-archrootfs/releases


Arch Linux official Docker image gitlab repository: https://gitlab.archlinux.org/archlinux/archlinux-docker

OCI-Compatible images for Arch Linux official:

https://hub.docker.com/_/archlinux

https://hub.docker.com/r/archlinux/archlinux/

https://quay.io/repository/archlinux/archlinux

https://github.com/archlinux/archlinux-docker/pkgs/container/archlinux
