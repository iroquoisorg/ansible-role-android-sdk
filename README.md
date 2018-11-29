# android-sdk

[![Build Status](https://travis-ci.com/iroquoisorg/ansible-role-android-sdk.svg?branch=master)](https://travis-ci.com/iroquoisorg/ansible-role-memcached)

Ansible role for android-sdk

This role was prepared and tested for Ubuntu 16.04.

# Installation

`$ ansible-galaxy install iroquoisorg.android-sdk`

# Default settings

```

# defaults file for android-sdk

android_sdk_download_location: http://dl.google.com/android/android-sdk_r24.4.1-linux.tgz
android_sdk_install_location: /opt
android_executable: "{{ android_sdk_install_location }}/android-sdk-linux/tools/android"

ubuntu_dependency_packages:
  - "unzip"
  - "libncurses5:i386"
  - "libstdc++6:i386"
  - "zlib1g:i386"
  - "imagemagick"
  - "expect"
  - "ant"
  - "ccache"
  - "autoconf"
  - "automake"
  - "ant"
  - "ccache"
  - "python-dev"
  - "zlibc"

ubuntu_precise_dependency_packages:
  - "libgd2-xpm"
  - "libgphoto2-2"
  - "libsane"
  - "ia32-libs-multiarch"

gradle_version: 4.1

rh_dependency_packages:
  - expect
  - libstdc++.i686
  - mesa-libGL-devel
  - ncurses-libs.i686
  - zlib.i686

android_sdk_update_path: true

android_sdk_base_buildtools_version: 26.0.2 # Used for PATH when android_sdk_update_path is true

android_sdk_tools_to_install:
  - "build-tools-{{ android_sdk_base_buildtools_version }}"
  - build-tools-19.1.0
  - build-tools-23.0.2
  - build-tools-25.0.1
  - build-tools-26.0.2
  - build-tools-27.0.1
  - platform-tools
  - tools
  - extra-android-support
  - extra-google-m2repository
  - extra-android-m2repository

android_sdks_to_install:
  - android-27
  - android-26
  - android-25
  - android-24
  - android-23
  - android-22
  - android-21
  - android-20
  - android-19
  - android-18
  - android-17
  - android-16

android_sdk_user: root

```
