# etaHEN - AIO Homebrew enabler

![etaHEN](https://github.com/LightningMods/etaHEN/blob/main/ETAHEN.png)

## Official PS5 exploit website (auto loads etaHEN)
- https://pkg-zone.com/exploit/PS5/index.html

## Features
 - Custom System Software version (custom System info)
 - kstuff for fself and fpkg support (4.5x and 4.03 only)
 - Debug Settings
 - HEN config file for settings
 - Jailbreak IPC call (jailbreaks Homebrew apps)
 - Update blocker (unmounts update partition)
 - libhijacker
 - *Optional* Illusions cheats/patches
 - *Optional* FTP server on port 1337
 - Klog server on port 9081
 - elf loader on port 9027
 - *Optional* PS5Debug
 - *started* Itemzflow intergration

## Upcoming features
 - More userland patches
 - (maybe) Jailbreak whitelist for Homebrew
 - plugin loader

## etaHEN INI Configuration file 
etaHEN's ini settings file can be found at `/data/etaHEN/config.ini` and can be accessed using the built-in FTP
and is automatically created when you run etaHEN for the first time

#### Configuration Layout 

| INI Key             | Description                                                 | Default value
|---------------------|-------------------------------------------------------------|---------------------|
| `libhijacker_cheats` | 0 = disables Illusions cheats  1 = enables Illusions cheats |  0 (disabled)     |                                         
| `PS5Debug`           | 0 = disables PS5Debug auto load 1 = enable PS5Debug auto load | 1 (enabled)     |
| `FTP`                | 0 = disables etaHEN built-in FTP 1 = enables it                | 1 (enabled)    |


## Contributors
- [sleirsgoevy](https://github.com/sleirsgoevy)
- [ChendoChap](https://github.com/ChendoChap)
- [astrelsky](https://github.com/astrelsky)
- [illusion](https://github.com/illusion0001)
- CTN & [SiSTR0](https://github.com/SiSTR0) for PS5Debug
- [Nomadic](https://github.com/jeroendev-one) for Dumper assistance 

## Testers
- [Echo Stretch](https://twitter.com/StretchEcho)
- [idlesauce](https://github.com/idlesauce)
- [Dizz](https://github.com/DizzRL)
- [BedroZen](https://twitter.com/BedroZen)
- [MODDED WARFARE](https://twitter.com/MODDED_WARFARE)

## Support the project
- https://ko-fi.com/lightningmods


## Join us on Discord
- https://discord.gg/xs2F46tKzK
