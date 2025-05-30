### ASUS-TUF-GAMING-B460M-PLUS-RX590
### The overall configuration list of my black Apple host is as follows:

| Part Type     | Part Model 
|---------------|----------------------------------------------|
| Opencore      |  1.0.5                                       |
| Version       |  macOS Sequoia15.5Beta3                      |
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
|--------------------------|
|  SSDT-AWAC               |
|  SSDT-Drop               |
|  SSDT-PLUG               |
|  SSDT-EC                 |
|  SSDT-RHUB               |
|  SSDT-USBX               |  


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
| CPUFriend.kext                        |
| RestrictEvents.kext                   |
| XHCI-unsupported.kext                 |
| RadeonSensor.kext                     |
| NVMeFix.kext                          |
| FeatureUnlock.kext                    | 
| HibernationFixup.kext                 | 
| cpuTscSync.kext                       | 
| IntelMausi.kext                       | 
| USBPorts.kext                         | 
| USBWakeFixup.kext                     | 
| IO80211FamilyLegacy.kext              | 
| IOSkywalkFamily                       |
| AirportItlwm-15.5Sequoia.kext         | 
| IntelBTPatcher.kext                   | 
| IntelBluetoothFirmware.kext           |
| BlueToolFixup.kext                    |
| AMFIPass.kext                         |
| RadeonBoost.kext                      |


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

## 关于打赏

如果您认可我的工作，请通过打赏支持我后续的更新(自觉打赏的人真少啊，免费的东西长久不了,现已改为需要密码解压，需微信或支付宝打赏入群。打赏记得留言备注你的qq号，然后申请入群时，填写你的留言为验证答案就是，我确认后会通过你的验证的。PS:之所以设置打赏，并不是为了赚大钱，当然大家打赏的多是有一些零花钱。主要是维护更新不易，每次系统一更新，有问题的话，就要工作时间之外花时间去调试，解决问题。普通群最多500人，无门槛的入群，不够用，有些机友对无门槛进入还不珍惜，进退群很随意，不看相关说明，上来就问问题的又多。不多说了，理解不理解的，就这样吧。

|  微信                                                                                 |
|---------------------------------------------------------------------------------------|
| ![1](https://github.com/user-attachments/assets/06d87fea-0d11-4bf4-b9ed-034dc7f53d06) | 
|                                                                                       |

若有其他问题请加Q群： 738882434
