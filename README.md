# etaHEN - AIO Homebrew enabler

![etaHEN](https://github.com/LightningMods/etaHEN/blob/main/ETAHEN.png)

## 🚀 **Support the Project**

If you find this project useful and would like to support its continued development, consider buying me a coffee!
[![ko-fi](https://www.ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/lightningmods)

## Official PS5 exploit website (auto loads etaHEN)
- https://ps5jb.pages.dev/

## Features
 - ★ etaHEN toolbox (debug settings replacement)
 - Custom etaHEN [Plugins](https://github.com/LightningMods/etaHEN-SDK/tree/main/Plugin_samples)
 - [Toolbox] Install the Homebrew Store on the console
 - [Toolbox] ★Rest Mode Options
 - [Toolbox] Blu-Ray license activation 
 - [Toolbox] etaHEN credits and supporters
 - [Toolbox] Auto open menu after etaHEN loads
 - 2 seperate daemons for improved stability and reliability
 - the Util daemon willl be auto restarted by the main etaHEN daemon
 - Custom System Software version (custom System info)
 - kstuff for fself and fpkg support 
 - etaHEN log in /data/etaHEN
 - (optional) System-wide controller shortcut to open itemzflow
 - Debug Settings
 - Game Dumper (Intrgrated with Itemzflow)
 - HEN config file for settings
 - Jailbreak IPC call (jailbreaks Homebrew apps)
 - Update blocker (unmounts update partition)
 - *Optional* Illusions cheats/patches [Plugin](https://github.com/LightningMods/etaHEN-SDK/tree/main/Plugin_samples/Illusion_cheats)
 - *Optional* FTP server on port 1337
 - *Optional* /data allowed inside apps sandboxes
 - Klog server on port 9081
 - elf loader on port 9027
 - *Optional* PS5Debug
 - *started* Itemzflow intergration
 - *Optional* Discord RPC server on port 8000, click [here](https://github.com/jeroendev-one/ps5-rpc-client) for setup instructions 
 - *Optional* Direct PKG installer service on port 9090

## etaHEN SDK
make your own custom plugins or payload-like ELFs for the HENV plugin via the [etaHEN SDK](https://github.com/lightningmods/etaHEN-SDK)
More info [Here](https://github.com/LightningMods/etaHEN-SDK/blob/main/README.md)

## Upcoming features
 - [Toolbox ONLY] load plugins without the HENV plugin
 - [Toolbox] FPS Counter
 - [Toolbox] change debug settings text
 - [Toolbox] On-Screen temps and other info
 - More userland patches
 - (maybe) Jailbreak whitelist for Homebrew
 - Improved PS5 Game support (itemzflow)
 - More (consider donating)

## etaHEN INI Configuration file 
etaHEN's ini settings file can be found at `/data/etaHEN/config.ini` and can be accessed using the built-in FTP
and is automatically created when you run etaHEN for the first time

#### Configuration Layout  (toolbox)
| INI Key             | Description                                                 | Default value
|---------------------|-------------------------------------------------------------|---------------------|                                        
| `PS5Debug`           | 0 = disables PS5Debug (Sistr0) auto load 1 = enable PS5Debug auto load  | 1 (enabled)    |
| `FTP`                | 0 = disables etaHEN built-in FTP 1 = enables it                | 1 (enabled)    |
| `discord_rpc`	       | 0 = disables Discord RPC server 1 = enables it 	        | 0 (disabled)   | 
| `testkit`	       | 0 = not testkit 1 = Real Testkits ONLY 	        | 0 (disabled)   | 
| `Allow_data_in_sandbox` | 0 = disables /data in an apps sandbox 1 = enables it 	        | 1 (enabled)   |
| `DPI`	       | 0 = disables The Direct PKG Installer service 1 = enables it 	        | 1 (enabled)   | 
| `Klog`               | 0 = disables kernel logging, 1 = enables it                  | 0 (disabled)   |
| `ALLOW_FTP_DEV_ACCESS` | 0 = disables FTP developer access, 1 = enables it           | 0 (disabled)   |
| `StartOption`        | 0=None, 1=Home menu, 2=Settings 3=Toolbox, 4=itemzflow            | 0 (None)    |
| `Rest_Mode_Delay_Seconds` | Delay in seconds before patching shellui coming out rest mode             | 0 (no delay)   |
| `Util_rest_kill`     | 0 = dont kill the util daemon during rest, 1 = Do kill it on rest     | 0 (disabled)   |
| `Game_rest_kill`     | 0 = dont kill the open game during rest, 1 = Do kill it  on rest         | 0 (disabled)   |

## DPI API details for tool creators 
etaHEN's Direct PKG Installer currently is very simple and is considered a WIP
the service flow is as follows

1. Connect to etaHEN's TCP server via port 9090 (using the PS5s IP)
2. Send a URL to etaHEN in the following json format
```
{ "url" : "http://xxxx" }
```
3. etaHEN will then send back the return value (0 on success)
```
{ "res" : "0" }
```
4. etaHEN will close the client socket after the return json is sent

## Contributors
- [sleirsgoevy](https://github.com/sleirsgoevy)
- [ChendoChap](https://github.com/ChendoChap)
- [astrelsky](https://github.com/astrelsky)
- [illusion](https://github.com/illusion0001)
- CTN & [SiSTR0](https://github.com/SiSTR0) for PS5Debug
- [SiSTR0](https://github.com/SiSTR0) for PS5Debug
- [Nomadic](https://github.com/jeroendev-one) (Discord RPC feature)

## Testers
- [Echo Stretch](https://twitter.com/StretchEcho)
- [idlesauce](https://github.com/idlesauce)
- [Dizz](https://github.com/DizzRL)
- [BedroZen](https://twitter.com/BedroZen)
- [MODDED WARFARE](https://twitter.com/MODDED_WARFARE)


## Join us on the Support Discord
- https://discord.gg/xs2F46tKzK
