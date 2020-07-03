# ryzentosh

> OpenCore 0.5.8 EFI for ASRock x570M Pro4 motherboard, macOS Catalina 10.15.5  
> AMD Radeon RX 5700XT, any AMD Ryzen 7/9 series CPU should work

## UEFI Settings

* Boot / CSM: disabled
* Boot / Above 4g decoding: enabled
* Disable SATA deep sleep
* Disable serial port

## What's working

* Everything except the things below

## What I'm still working on

* Inject PowerPlayTable data to undervolt and overclock the GPU
* Display correct CPU name in System Information
* GUI for boot menu

## What doesn't work

* Front panel mic (will never work)
* Hyperkit (just use docker toolbox with VirtualBox)
* DRM in Safari and TV (DRM in Firefox/Chrome works fine)
