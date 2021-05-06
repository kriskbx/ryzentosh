# ryzentosh

> OpenCore 0.6.6 EFI for ASRock x570M Pro4 motherboard, macOS Big Sur 11.2
> AMD Radeon RX 5700XT, any AMD Ryzen Zen series CPU should work (I'm using a Ryzen 9 5900)

## Bios

I updated to v3.0 with a Pinnacle Ridge CPU [using this guide](https://download.asrock.com/TSD/Ryzen5000/X570M%20Pro4.pdf). Then exchanged the CPU to a 5000 series and upgraded normally to v3.4.

## UEFI Settings

* Disable CSM
* Enable Above 4g decoding
* Disable SATA deep sleep
* Disable serial port
* Disable Thunderbolt
* Enable Resizable Bar for better graphics performance

## What's working

* Sleep/Hibernation!
* Everything except the things below

## What's kinda working

* USB accessories on the second USB controller (XHCI, formerly XHC1) sometimes freeze the system when under heavy load. USB-mapping was done correctly (I checked four times) and the Embedded Controller and USB-X fix for power management seems to work reliably too. Not really sure what's causing this. For now I just use the USB ports on the second and third row, as well as the frontside ports.

## What doesn't work

* Display of correct CPU name in System Information (hard to do without disabling sip)
* Front panel mic (will never work)
* Hyperkit (use docker toolbox with VirtualBox)
* DRM in Safari and Apple TV (DRM in Firefox/Chrome works fine)
