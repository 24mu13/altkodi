# AltStore Source for Kodi

This source provide a way to install Kodi on iOS devices using AltStore. 
It is a simple and easy way to get Kodi on your iOS device without the need for a computer.

![Kodi](https://raw.githubusercontent.com/xbmc/xbmc/refs/heads/master/media/icon48x48.png)

## How to use

1. Install [AltStore](https://altstore.io/) or [SideStore](https://github.com/SideStore/SideStore) on your iOS device.
2. Add this source to the store: 
   `https://24mu13.github.io/altkodi/apps.json`
3. Search for **Kodi** in the store and install it.

**Note**: using **SideStore** is not yet working automatically because of https://github.com/SideStore/SideStore/issues/227, but you could work around as follows:
- Download the IPA file manually and remove both .o files in the path `Payload/Kodi.app/Frameworks/lib/python3.11/config-3.11-darwin/`
- Copy the tweaked file to the device
- Install it using SideStore → My Apps → +

### SideStore

If you are going to use **SideStore**, you need to install the app as described [here](https://docs.sidestore.io/docs/installation/prerequisites).

In short, as per today (January 2026):
- Install [LocalDevVPN](https://apps.apple.com/us/app/localdevvpn/id6755608044) on device and connect the VPN
- Install [iloader](https://github.com/nab138/iloader) on computer
- Connect device to computer via USB and run `iloader` to install SideStore

## Other manual installation methods

## iloader

See https://github.com/nab138/iloader

## Sideloader (Linux)

1. Install [Sideloader](https://github.com/Dadoum/Sideloader)
2. Download or generate the IPA file for Kodi (see https://kodiipa.com)
3. Install Kodi using the following command
   `sideloader-cli-x86_64-linux-gnu install kodi.ipa -i`

## Sideloadly (Windows or Mac)

Use **Sideloadly** as described in the official reference below.

## References
- [Kodi IPA](https://kodiipa.com)
- [Install Kodi for iOS](https://kodi.wiki/view/HOW-TO:Install_Kodi_for_iOS)
- [AltStore](https://altstore.io/)
