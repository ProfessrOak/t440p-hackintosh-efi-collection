This Github repo is for people who want to install MacOS Ventura on their Thinkpad T440p. I couldn't find anyone else who uploaded their EFI folder for Ventura to Github, so I think I may be the first one. Enjoy!
But first though, you'll have to use GenSMBIOS to generate an SMBIOS (by first selecting the config.plist file) for MacBookPro14,1 or 15,1, then use ProperTree to insert your MAC address at PlatformInfo -> Generic -> ROM (also by selecting the config.plist file)



Here's how to make it bootable:
1. Decompress Audio.zip
2. Create a folder called "Resources"
3. Move the Font, Audio, Image, and Label folders into the Resources folder.
4. Create a folder called "OC"
5. Move every folder except for the "Boot" folder into "OC"
6. Modify the info.plist file by following the intructions above.
7. And finally, create the EFI folder itself, then drag the BOOT and OC folders into it. You should now have an EFI folder that you can use to boot MacOS Ventura.



The reason why I had to do this was because github wouldn't let me upload more than 100 files at a time, for those curious.



*If you're using the stock trackpad and not the T450/ X1 Carbon 3rd gen trackpad, then your trackpad may not work. I haven't tested it yet with the stock trackpad.

*You'll need to use OpenCore Legacy Patcher to first patch the installation media by clicking on "Create macOS installer", then run it again after booting into Ventura. The reason why this is required is because Ventura doesn't have any native support for HD 4600 graphics.
