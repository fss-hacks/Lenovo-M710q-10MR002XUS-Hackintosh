This is the EFI for the Lenovo M710q Tiny version 10MR002XUS.
System specs:
Core i3-7100T (2C, 3.4GHz, 3MB) Kaby Lake (Being run as MacMini8,1)
Integrated Intel HD Graphics 630
128GB SSD M.2 PCIe NVMe (Runs slowly, WIP)
Intel 3165 ac, 1x1 + BT4.1 (AirportItlwm and BlueToolFixup take care of this)
OpenCore 1.0.0 EFI at time of writing, update to latest OpenCore at your own peril.
Running reliably on Mac OS Monterey (this is the best OS version due to speed and compatibility issues - the same EFI can run Big Sur and Ventura but Big Sur has issues with applications being supported and Ventura runs extremely slowly due to the hardware specs)

What is working:
Everything except for iServices. As of right now, DO NOT sign into your Apple ID or try to use the App Store, it causes a kernel panic/bootloop and the drive will need to be wiped and OS reinstalled.

Instructions:
Download the EFI .zip file and prepare an OpenCore USB boot drive with your Mac OS installer files.
The EFI comes without SMBIOS info in it so you will need to edit the config.plist with ProperTree or OPCAT etc and input a generated serial that matches MacMini8,1.

