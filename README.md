This Github repo contains the EFI folder required to boot Mac OS Ventura 13.4 on your Thinkpad T440p. Please note that you will need to generate your own SMBIOS for MacBookPro14,1 or 15,1 (if you want to ensure future compatibility with Mac OS Sonoma) using GenSMBIOS, and if you're using the stock trackpad instead of the T450/T450s/X1 Carbon 3rd Gen trackpad, I'm not sure if it will work. If you're using the stock trackpad, clone Valnoxy's repo (linked below), copy VoodooPS2Controller.kext and VoodooRMI.kext from the EFI/OC/Kexts folder for Monterey, copy them over to the same folder in this repo, then click on replace when prompted. Then use OC Auxillary Tools to update the two kext files so that they work on Ventura. Last but not least, you will need to edit the config.plist file with your MAC address (without the dashes) using ProperTree in the PlatformInfo -> Generic -> ROM section. This step is crucial for working iMessage, so DON'T skip it!


Post Install:
Use OpenCore Legacy Patcher to patch your Ventura install. This is because Apple dropped support for HD 4600 graphics with Mac OS Ventura, and unless you want a painfully
slow experience on Mac OS, then this step is required.

This repo is mostly based off this [repo](https://github.com/valnoxy/t440p-oc). The only differences are that this repo has updated kext files for OpenCore 0.9.3 and Ventura as well as the kext files required for scrolling to work on the 3 button trackpad (Synaptics).
