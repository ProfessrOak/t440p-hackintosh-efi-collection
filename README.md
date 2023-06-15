This Github repo contains the EFI folder required to boot Mac OS Ventura 13.4 on your Thinkpad T440p. Please note that you will need to generate your own SMBIOS for MacBookPro14,1 or 15,1 using GenSMBIOS, and if you're using the stock trackpad instead of the T450/T450s/X1 Carbon 3rd Gen trackpad, I'm not sure if it will work. Last but not least, you will need to edit the config.plist file with your MAC address using ProperTree in the PlatformInfo -> Generic -> ROM section. This step is crucial for working iMessage, so DON'T skip it!


Post Install:
Use OpenCore Legacy Patcher to patch your Ventura install. This is because Apple dropped support for HD 4600 graphics with Mac OS Ventura, and unless you want a painfully
slow experience on Mac OS, then this step is required.

