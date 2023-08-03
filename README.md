# unofficial-archrootfs

<p align="left">
  <img src="https://github.com/Zhoneym/unofficial-archrootfs/assets/140673973/a1f7322b-b56e-4696-9d1b-9487121b02aa" width="75"/>
</p> 

[![Build Arch Linux rootfs](https://github.com/Zhoneym/unofficial-archrootfs/actions/workflows/build.yml/badge.svg)](https://github.com/Zhoneym/unofficial-archrootfs/actions/workflows/build.yml)


This is an unofficial packaging that complies with the OCI standard rootfs and is also applicable to Microsoft WSL2. Originally intended to temporarily replace the construction of the official Docker image in the event of issues with the official Gitlab-CI build，but it is still a relatively ideal choice


Arch Linux, a lightweight and flexible Linux® distribution that tries to Keep It Simple.

Compared to the official Docker image repository, this repository has the following advantages:


 - Faster update frequency
 - A simpler and more transparent packaging method
 - High degree of freedom and customizability


We offer three options:


 - base: Minimal package set to define a basic Arch Linux installation
 - base-devel: Minimum package set to define a basic Arch Linux installation and basic tools to build Arch Linux packages
 - workstations: Contains commonly used compiler tools and common system management tools (this option is very suitable for working with Microsoft WSL2)
