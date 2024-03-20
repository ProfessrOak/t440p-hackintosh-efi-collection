Contains the EFI folders needed to boot Macos Sonoma on your Thinkpad T440p. There are two, with the only difference between them being airportitlwm.kext. This is because the airportitlwm kext for 14.0 to 14.3.1 will not work on 14.4 and above. iServices like iMessage won't work. YMMV, but using itlwm instead may fix these issues.

You will need to use [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) to generate a valid serial for MacBookPro16,1, as that is the SMBIOS the USB map is for.

The SD card reader will not work as I haven't found a compatible kext

Use [OCPL](https://github.com/dortania/OpenCore-Legacy-Patcher) to make your experience usable, as Sonoma doesn't support Haswell igpus

ACPI patches by [valnoxy](https://github.com/valnoxy)

