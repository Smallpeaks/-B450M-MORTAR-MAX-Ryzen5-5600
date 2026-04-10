## MSi-B450M-MORTAR-MAX
### MSi-B450M-MORTAR-MAX-Ryzen5-5600-RX6650XT-OC1.0.8
### The overall configuration list of my black Apple host is as follows:

| Part Type     | Part Model 
|---------------|----------------------------------------------|
| Opencore      |  1.0.8                                       |
| Version       |  macOS Sequoia15.7-26.4                      |
| Motherboard   |  MSi-B450M-MORTAR-MAX                        |
| Hard disk     |  KPART512GBC2DVT M2                          |
| Graphics      |  RX6650XT 8G                                 |
| CPU           |  AMD Ryzen 5 5600 6-Core Processor           |
| Memory        |  ADATA 16GB DDR4 3200MHz(8GB + 8GB)          |
| Wireless      |  Realtek PCle GbE Family / ntel AX210        |
| Radiator      |  Kaneda 9cm six-tube copper fan              |
| Power supply  |  600W for the journey                        |
| Chassis       |  LOVINGCOOL Ocean View Room                  |
| sound card    |   Realtek® ALC892/ALC897 Codec      alcid=1  |

MSi-B450M-MORTAR-MAX Series Motherboards MacOS 15.7-26.4 Completeness:

Front-end and back-end sound output normal

All USB ports normal

Wired internet/WIFI normal
 
iMessage、FaceTime normal

Hardware acceleration of the GPU normal

Sleep/wake up normal

The built-in microphone is normal

It's normal to wake up from sleep

Solution 1: The onboard intel AX210 Bluetooth and WIFi can be driven, and the network speed is very good, but it does not support air-car. MacOS 15 requires the HELIPORT APP to use the WIFI function

Solution 2: The onboard intel AX210 Bluetooth and WIFi can be driven, and the network speed is very good, but it does not support air-carry; MacOS 15.7-26.4 requires OCLP patching here using option 2

If you want to achieve the additional function of air carry, you need to buy a NVME M.2 SSD to connect to the Heiguo wireless network card

The boot can support independent graphics (RX560/570/590/5500/5600/5700/6600/6650 and other series) by default.

I won't talk about them one by one

### OpenCore Configuration

### ACPI

| ACPIs                    |
|--------------------------|
|  SSDT-EC                 |
|  SSDT-PMC                |

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
| NootRX.kext                           |
| SMCProcessor.kext                     |
| AppleALC.kext                         |
| RestrictEvents.kext                   |
| NVMeFix.kext                          |
| AppleMCEReporterDisabler.kext         | 
| HibernationFixup.kext                 | 
| AMDRyzenCPUPowerManagement.kext       | 
| FeatureUnlock.kext                    | 
| RealtekRTL8111.kext                   | 
| IO80211FamilyLegacy.kext              | 
| IOSkywalkFamily                       |
| AirportItlwm-15.5Sequoia.kext         | 
| IntelBTPatcher.kext                   | 
| IntelBluetoothFirmware.kext           |
| BlueToolFixup.kext                    |
| AMFIPass.kext                         |
| RadeonBoost.kext                      |
| USBXHCI.kext                          |     
| USBInjectAll.kext                     |   

## BIOS recommended settings

  Advanced -- Configuration  -- changed to CSMUEFI

  Advanced -- Configuration  -- Secure boot -- Disable secure boot (disable by default)

  Advanced -- USB settings -- XHCI Hand-off -- On (on by default)

 ## 若有其他问题请加Q群： 738882434
  
