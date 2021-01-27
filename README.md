# zigpy-deconz

[![Build Status](https://travis-ci.org/zigpy/zigpy-deconz.svg?branch=master)](https://travis-ci.org/zigpy/zigpy-deconz)
[![Coverage](https://coveralls.io/repos/github/zigpy/zigpy-deconz/badge.svg?branch=master)](https://coveralls.io/github/zigpy/zigpy-deconz?branch=master)

[zigpy-deconz](https://github.com/zigpy/zigpy-deconz) is a Python 3 implementation for the [Zigpy](https://github.com/zigpy/) project to implement support for [Zigbee](https://www.zigbee.org) radio devices that uses firmware with [deCONZ serial protocol](https://github.com/dresden-elektronik/deconz-serial-protocol).

The goal of this project for [zigpy](https://github.com/zigpy/) is to add support for [ConBee](https://phoscon.de/en/conbee/), [ConBee II (ConBee 2)](https://phoscon.de/en/conbee2/), and [RaspBee](https://phoscon.de/en/raspbee2/) and [RaspBee II](https://phoscon.de/en/raspbee2/) Zigbee adapters/modules from [Dresden-Elektronik](https://github.com/dresden-elektronik/) to integrations such as [ZHA in Home Assistant](https://www.home-assistant.io/integrations/zha/).

# Testing new releases

Testing a new release of the zigpy-deconz library before it is released in Home Assistant.

If you are using Supervised Home Assistant (formerly known as the Hassio/Hass.io distro):
- Add https://github.com/home-assistant/hassio-addons-development as "add-on" repository
- Install "Custom deps deployment" addon
- Update config like: 
  ```
  pypi:
    - zigpy-deconz==0.9.0
  apk: []
  ```
  where 0.5.1 is the new version
- Start the addon

If you are instead using some custom python installation of Home Assistant then do this:
- Activate your python virtual env
- Update package with ``pip``
  ```
  pip install zigpy-deconz==0.9.0

# Releases via PyPI
Tagged versions are also released via PyPI

- https://pypi.org/project/zigpy-deconz/
- https://pypi.org/project/zigpy-deconz/#history
- https://pypi.org/project/zigpy-deconz/#files

# External documentation and reference

Note! Latest official documentation for the deCONZ serial protocol can currently be obtained by contacting Dresden-Elektronik employees via GitHub here:
- https://github.com/dresden-elektronik/deconz-serial-protocol
  - https://github.com/dresden-elektronik/deconz-serial-protocol/issues/2

For reference, here is a list of unrelated projects that also use the same deCONZ serial protocol for other implementations
- https://github.com/Equidamoid/pyconz/commits/master
- https://github.com/mozilla-iot/deconz-api
- https://github.com/adetante/deconz-sp
- https://github.com/frederic34/plugin-nodeBee

# How to contribute

If you are looking to make a contribution to this project we suggest that you follow the steps in these guides:
- https://github.com/firstcontributions/first-contributions/blob/master/README.md
- https://github.com/firstcontributions/first-contributions/blob/master/github-desktop-tutorial.md

Some developers might also be interested in receiving donations in the form of hardware such as Zigbee modules or devices, and even if such donations are most often donated with no strings attached it could in many cases help the developers motivation and indirect improve the development of this project.
