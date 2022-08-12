# ASUS Z690 ProArt Creator WiFi-Hackintosh-OC8.0
ASUS Z690 ProArt Creator WiFi Hackintosh-macOS Monterey-OpenCore

# Configuration

## 硬件配置 / Specifications:

Motherboard：ASUS Z690 ProArt Creator WiFi
CPU：Intel i9-12900K
RAM：Kingston Fury beast DDR5 5600 32GB X2
GPU：Radeon™ RX 6900 XT 16G
SSD：WD BK SN850 1TB



## BIOS设定 / ASUS Z690 ProArt Creator WiFi BIOS Setting

- Exit → Load Optimized Defaults
- Ai Tweaker
  - Ai Overclock Tuner → XMP I (or select XMP II to test different memory overclock modes)
- Advanced → CPU Configuration
  - Option 1: To enable all cores, all threads, but limit max CPU frequency to that of E-cores
    - Active Performance Cores → All
    - Active Efficient Cores → All
    - Hyper-Threading → Enabled
  - Option 2: To disable E-cores for maximum P-core frequencies
    - Active Performance Cores → All
    - Active Efficient Cores → 0
    - Hyper-Threading → Enabled
- Advanced → System Agent Configuration
  - VT-d → Enabled
- Advanced → System Agent Configuration → Memory Configuration
  - Memory Remap → Enabled (enables Above 4G Decoding)
- Advanced → System Agent Configuration → Graphics
  - Primary Display → PEG Slot
  - iGPU Multi Monitor → Disabled (optionally, this can be enabled)
- Advanced → Thunderbolt Configuration
  - PCIE Tunneling over USB4 → Enabled
  - Discrete Thunderbolt(TM) Support → Enabled
  - Wake From Thunderbolt(TM) Devices → Enabled
- Advanced → Thunderbolt Configuration → Discrete Thunderbolt(TM) Configuration
  - DTBT Go2Sx Command → Enabled
  - Windows 10 Thunderbolt support → Enable + RTD3
- Advanced → Trusted Computing
  - Security Device Support → Enable
- Advanced → PCI Subsystem Settings
  - Re-Size BAR Support → Enabled (if your GPU supports it) or it can be Disabled
    - If Enabled, set ResizeAppleGpuBars to 0 in Booter section of config.plist
- Advanced → USB Configuration
  - XHCI Hand-off → Enabled
- Advanced → Network Stack Configuration
  - Network Stack → Disabled
- Advanced → Onboard Devices Configuration
  - HD Audio → Enabled
  - Intel LAN → Enabled
  - MARVELL 10G LAN → Enabled
  - USB power delivery in Soft Off state (S5) → Enabled (can be Disabled to turn off USB devices)
  - Wi-Fi Controller → Disabled (to use Intel WiFi set to Enabled)
  - Bluetooth Controller → Disabled (to use Intel Bluetooth set to Enabled)
  - Serial Port Configuration → Disabled
- Boot → Boot Option Priorities
  - If there are multiple bootable disks in the system, configure the boot priority order
- Boot → CSM (Compatibility Support Module)
  - Launch CSM → Disabled
- Boot → Secure Boot
  - OS Type → Other
  - Secure Boot Mode → Custom
- Boot → Boot Configuration
  - Fast Boot → Enabled (or choose Disabled)
- Tool → ASUS User Profile
  - Profile Name → (Enter name of profile in order to save current BIOS configuration)
  - Save to Profile → (Up to 8 profiles can be saved)
- Exit
  - Save Changes & Reset (choose this option when BIOS configuration is done)

### Short List:

From default EZ Mode screen, enable X.M.P. then select Advanced Mode (F7) as shown: 
BIOS 01 EZ Mode.jpg


- Exit → Load Optimized Defaults
- Advanced → CPU Configuration
  - Option 1: To enable all cores, all threads, but limit max CPU frequency to that of E-cores
    - Active Performance Cores → All
    - Active Efficient Cores → All
    - Hyper-Threading → Enabled
  - Option 2: To disable E-cores for maximum P-core frequencies
    - Active Performance Cores → All
    - Active Efficient Cores → 0
    - Hyper-Threading → Enabled
- Advanced → System Agent Configuration
  - VT-d → Enabled
- Advanced → System Agent Configuration → Graphics
  - Primary Display → PEG Slot
  - iGPU Multi Monitor → Disabled (optionally, this can be enabled)
- Advanced → PCI Subsystem Settings
  - Re-Size BAR Support → Enabled (if your GPU supports it) or it can be Disabled
    - If Enabled, set ResizeAppleGpuBars to 0 in Booter section of config.plist
- Advanced → Onboard Devices Configuration
  - Wi-Fi Controller → Disabled (to use Intel WiFi set to Enabled)
  - Bluetooth Controller → Disabled (to use Intel Bluetooth set to Enabled)
  - Serial Port Configuration → Disabled
- Boot → Boot Option Priorities
  - If there are multiple bootable disks in the system, configure the boot priority order
- Boot → Secure Boot
  - OS Type → Other
  - Secure Boot Mode → Custom
- Boot → Boot Configuration
  - Fast Boot → Enabled (or choose Disabled)
- Tool → ASUS User Profile
  - Profile Name → (Enter name of profile in order to save current BIOS configuration)
  - Save to Profile → (Up to 8 profiles can be saved)
- Exit
  - Save Changes & Reset (choose this option when BIOS configuration is done)
- Exit → Load Optimized Defaults
