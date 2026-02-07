# MiSTer FPGA - Smart Launcher

<img src="docs/images/1.png" alt="drawing" width="500"/>

## Overview
**MiSTeR FPGA - Smart Launcher** is an application for MiSTer FPGA that lets you easy browse your ROM set, filter it, and launch games from any device (PC/Smart Phone/Tablet) through a web browser.<br>
It creates a very lightweight web server under the hood.

## Before Installation
The application uses a database containing all the information about the ROM set you are using on MiSTer.
To generate the database, you need to use the appication **MiSTeR FPGA - Smart Scanner**.
You can find all the informations [here](https://github.com/gerrykeys/MiSTer-FPGA_Smart-Scanner).

## Installation
Once you have generated the database, follow the steps below:

- Copy the application folder in `/media/fat/Scripts`
- Copy the `database` folder inside the installation folder `/media/fat/Scripts/MiSTer-Smart-Launcher`
- On the MiSTer, go to the Scripts menu and enter the installation folder.
- Select the file `run.sh`

Once this is done, you can access it from any browser at the following address:

`http://<YOUR-MISTER-IP>:8282`

Remember: if you reset the MiSTer, you will need to launch "run.sh" again.
In the future, there will be the option to install/uninstall the script as a service,
so that it starts automatically every time the MiSTer powers on or is reset.

## Suported Systems
The followings systems are supported (More systems will be available in future)

| Systems                         | Core (RBF)            | Supported formats                                 |
| --------------------------------|:---------------------:|:-------------------------------------------------:|
| Amiga                           | _Computer/Minimig     | .adf                                              |
| Amstrad                         | _Computer/Amstrad     | .dsk .e?? .cdt                                    |
| Apple II                        | _Computer/Apple-II    | .nib .dsk .do .po .hdv                            |
| Arcade                          | _Arcade/cores         | .mra                                              |
| Atari 2600                      | _Console/Atari7800    | .a78 .a26 .bin                                    |
| Atari 5200                      | _Console/Atari5200    | .car .a52 .bin .rom                               |
| Atari 7800                      | _Console/Atari7800    | .a78 .bin                                         |
| Atari 800                       | _Computer/Atari800    | .atr .xex .atx .xfd .car .rom .bin                |
| Atari Lynx                      | _Console/AtariLynx    | .lnx .lyx                                         |
| Coleco Vision                   | _Console/ColecoVision | .col .bin .rom                                    |
| Commodore 64                    | _Computer/C64         | .d64 .g64 .t64 .d81 .prg .crt .reu .tap           |
| Commodore VIC20                 | _Computer/VIC20       | .d64 .g64 .prg .crt .ct? .tap .rom                |
| Nintendo Game Boy               | _Console/Gameboy      | .gb                                               |
| Nintendo Game Boy Advance       | _Console/GBA          | .gba                                              |
| Nintendo Game Boy Color         | _Console/Gameboy      | .gbc                                              |
| Sega Genesis                    | _Console/Genesis      | .bin .gen .md                                     |
| Sega Master System              | _Console/SMS          | .sms                                              |
| Sega Mega Drive                 | _Console/MegaDrive    | .bin .gen .md                                     |
| MSX 1                           | _Computer/MSX1        | .rom                                              |
| Neo Geo                         | _Console/NeoGeo       | .neo                                              |
| Nintendo / Famicom              | _Console/NES          | .nes                                              |
| Nintendo 64                     | _Console/N64          | .z64 .n64                                         |
| Sony Playstation                | _Console/PSX          | .cue .bin .img .chd                               |
| Sega Saturn                     | _Console/Saturn       | .cue .bin .img .chd                               |
| Sega Mega CD                    | _Console/MegaCD       | .chd                                              |
| Super Nintendo / Super Famicom  | _Console/SNES         | .sfc                                              |
| Spectrum                        | _Computer/ZX-Spectrum | .trd .img .dsk .mgt .tap .csw .tzx .z80 .sna .vhd |
| PC Engine / Turbo Grafx16       | _Console/TurboGrafx16 | .bin .pce                                         |
| PC Engine CD / Turbo Grafx16 CD | _Console/TurboGrafx16 | .cue .bin .img .chd                               |
| Vectrex                         | _Console/Vectrex      | .vec .bin .rom                                    |
| Sharp X68000                    | _Computer/X68000      | .d88 .hdf .ram                                    |

## Roms in .Zip archive
ROMs with compatible extensions and compressed in .zip format are supported.<br>
Generally, MiSTer cores do not support the .zip format.
However, when MiSTer is used through the native UI interface, it can browse archives as if they were folders and allows selecting the ROM to launch.
When this happens, MiSTer handles unpacking the ROM and provides it as input to the relevant core.
**MiSTer FPGA – Smart Launcher** application therefore handles the unpacking of zip files in the same way.<br>


<img src="docs/images/2.png" alt="drawing" width="500"/>
