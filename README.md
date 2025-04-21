### ASUS-TUF-GAMING-B460M-PLUS-RX590
### The overall configuration list of my black Apple host is as follows:

| Part Type     | Part Model 
|---------------|----------------------------------------------|
| Opencore      |  1.0.5                                       |
| Version       |  macOS Sequoia15.4                           |
| Motherboard   |  ASUS TUF Gaming B460M PLUS                  |
| Hard disk     |  Coiorful CN600 1T M2                        |
| Graphics      |  RX590 8G                                    |
| CPU           |  Intel i7 10700                              |
| Memory        |  ADATA 2933 16G*2 DDR4                       |
| Wireless      |  network card: ntel AX210                    |
| Radiator      |  Kaneda 9cm six-tube copper fan              |
| Power supply  |  700W for the journey                        |
| Chassis       |  LOVINGCOOL Ocean View Room                  |


Support the full range of CPU models,  i5-10400, i7-10700, i9-10900K, i5-10200H, etc

ASUS-TUF-GAMING-B460M-PLUS Series Motherboards MacOS 15.4 Completeness:

CPU Normal Turbo Frequency (i5/i7/i9/etc.)

Onboard audio is normal

The graphics card supports HDMI/DP display output

The front and rear 3.5 audio outputs are normal

Sleep wake-up is normal

The wired NIC Intel® I219-V is in normal use

Solution 1: The onboard intel AX210 Bluetooth and WIFi can be driven, and the network speed is very good, but it does not support air-car. MacOS 15 requires the HELIPORT APP to use the WIFI function

Solution 2: The onboard intel AX210 Bluetooth and WIFi can be driven, and the network speed is very good, but it does not support air-carry; MacOS 15 requires OCLP patching here using option 2

If you want to achieve the additional function of air carry, you need to buy a NVME M.2 SSD to connect to the Heiguo wireless network card

The boot can support independent graphics (RX560/570/590/5500/5600/5700/6600 and other series) by default.

I won't talk about them one by one

### OpenCore Configuration

### ACPI

| ACPIs                                    |
|------------------------------------------|
|  SSDT-AWAC-ASUS-B460M-PLUS               |
|  SSDT-BIOS-ASUS-B460M-PLUS               |
|  SSDT-PLUG-ASUS-B460M-PLUS               |
|  SSDT-RMNE-ASUS-B460M-PLUS               |
|  SSDT-RHUB-ASUS-B460M-PLUS               |


### Drivers

| Driver Name     |
|-----------------|
| HfsPlus         |
| OpenCanopy      |
| OpenRuntime     |
| ResetNvramEntry |
| ToggleSipEntry  |

### Kexts


| Kext Name                             |
|---------------------------------------|
| Lilu.kext                             |
| VirtualSMC.kext                       |
| WhateverGreen.kext                    |
| SMCProcessor.kext                     |
| SMCSuperIO.kext                       |
| AppleALC.kext                         |
| AppleMCEReporterDisabler.kext         |
| RestrictEvents.kext                   |
| SMCRadeonGPU.kext                     |
| RadeonSensor.kext                     |
| NVMeFix.kext                          |
| FeatureUnlock.kext                    | 
| HibernationFixup.kext                 | 
| RTCMemoryFixup.kext                   | 
| LucyRTL8125Ethernet.kext              | 
| USBPorts.kext                         | 
| USBWakeFixup.kext                     | 
| IO80211FamilyLegacy.kext              | 
| IOSkywalkFamily                       |
| AirportItlwm-15.5Sequoia.kext         | 
| IntelBTPatcher.kext                   | 
| IntelBluetoothFirmware.kext           | 
| BlueToolFixup.kext                    | 

### BIOS Setup Reference:

Advanced \ CPU Configuration \ Software Guard Extensions (SGX): Software Controlled

Advanced \ CPU Configuration \ Intel (VMX) Virtualization Technology: Disabled

Advanced \ System Agent (SA) Configuration \ VT-d: Disabled

Advanced \ System Agent (SA) Configuration \ Graphics Configuration \ Primary Display: Auto

Advanced \ System Agent (SA) Configuration \ Graphics Configuration \ iGPU Multi-Monitor: Enabled

Advanced \ System Agent (SA) Configuration \ Graphics Configuration \ DVMT Pre-Allowcated: 256M

Advanced \ System Agent (SA) Configuration \ Graphics Configuration \ Primary Display: Auto

Advanced \ PCI Subsystem Settings \ Above 4G Decoding: Enabled

Advanced \ PCI Subsystem Settings \ SR-IOV Support: Disabled

Advanced \ USB Configuration \ XHCI Hand-off: Enabled

Advanced \ Onboard Devices Configuration \ Serial Port Configuration \ Serial Port: Off

Boot \ CSM (Compatibility Support Module) \ Lauch CSM: Disabled

Boot \ Secure Boot \ OS Type: Other OS

Boot \ Boot Configuration \ Fast Boot: Enabled

若有其他问题请加Q群： 738882434
