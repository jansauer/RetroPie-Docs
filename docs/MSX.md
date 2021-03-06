***
![msx2](https://cloud.githubusercontent.com/assets/10035308/12213189/80192ed2-b631-11e5-86b3-58d17dcc2432.png)
***
_The MSX was a 8bit personal computer standard developed by ASCII in 1983. Microsoft provided the BASIC interpreter and later MSX-DOS. Various electronics vendors made MSX systems such as Canon, Casio, Daewoo, Fujitsu, Goldstar (LG), Hitachi, JVC, Mitsubishi, Panasonic, Philips, Pioneer, Samsung, Sanyo, Sony, Toshiba, Yamaha and various others. The MSX was followed by the MSX2, after which manufacturers abandoned the market outside Japan due to limited success. In Japan a few manufacturers still held out and released the MSX2+ and finally the TurboR. MSX had its greatest success in Japan, and was able to establish some market share in countries like the Netherlands, Spain and Brazil._

***

| Emulator | Rom Folder | Extension | BIOS |  Controller Config |
| :---: | :---: | :---: | :---: | :---: |
| [lr-bluemsx](https://github.com/libretro/blueMSX-libretro) | msx  | .rom .mx1 .mx2 .col .dsk .m3u .zip | see below  | /opt/retropie/configs/msx/retroarch.cfg |
| [lr-fmsx](https://github.com/libretro/fmsx-libretro) | msx  | .rom .mx1 .mx2 .col .dsk | see below | /opt/retropie/configs/msx/retroarch.cfg |
| [OpenMSX](http://openmsx.org/) | msx | .rom .mx1 .mx2 .col .dsk | see below | hardcoded |

## Emulator: [lr-fmsx](https://github.com/libretro/fmsx-libretro), [lr-bluemsx](https://github.com/libretro/blueMSX-libretro), [OpenMSX](http://openmsx.org/)

## ROMS
Accepted File Extensions: **.rom .mx1 .mx2 .col .dsk .m3u (lr-blueMSX only) **

Place your MSX ROMs in
```
/home/pi/RetroPie/roms/msx
```

## Controls
 
lr-fmsx and lr-bluemsx utilise RetroArch configurations. openMSX has its own configuration, and will ignore control definitions made in RetroArch.

Add custom retroarch controls to the retroarch.cfg file in

```
/opt/retropie/configs/msx/retroarch.cfg
```

keyboard support can also be enabled here by adding:

```
input_libretro_device_p2 = "3"
```

For more information on custom RetroArch controls see: [RetroArch Configuration](RetroArch-Configuration)

Many games will have varying keyboard controls.


## BlueMSX BIOS

Depending on the CORE option and machine you are running, it may require a different BIOS. Each machine folder has an ini file that explains which BIOS is needed, the following are some examples.

## BlueMSX BIOS List

* COL - ColecoVision: coleco.rom
* MSX : MSX.ROM - PHILIPSDISK.ROM 
* MSX Brazilian : MSXBR.ROM - MICROSOLDISK.ROM 
* MSX German : MSXG.ROM - PHILIPSDISK.ROM 
* MSX Japanese : MSXJ.ROM - PANASONICDISK.ROM 
* MSX Korean : MSXKR.ROM - MSXHAN.ROM - NATIONALDISK.ROM 
* MSX Swedish : MSXSE.ROM - PHILIPSDISK.ROM 
* MSX2 : MSX2.ROM - MSX2EXT.ROM - MSX2PMUS.ROM - MOONSOUND.ROM - XBASIC2.ROM - PHILIPSDISK.ROM 
* MSX2 Arabic : MSX2AR.ROM - MSX2AREXT.ROM - MSX2PMUS.ROM - MOONSOUND.ROM - XBASIC2.ROM - PANASONICDISK.ROM - KANJI.ROM - MSXKANJI.ROM - ARABIC.ROM - SWP.ROM - PAINT.ROM 
* MSX2 Brazilian : MSX2BR.ROM - MSX2BREXT.ROM - MSX2PMUS.ROM - MOONSOUND.ROM - XBASIC2.ROM - MICROSOLDISK.ROM 
* MSX2 French : MSX2FR.ROM - MSX2FREXT.ROM - MSX2PMUS.ROM - MOONSOUND.ROM - XBASIC2.ROM - PHILIPSDISK.ROM 
* MSX2 German : MSX2G.ROM - MSX2GEXT.ROM - MSX2PMUS.ROM - MOONSOUND.ROM - XBASIC2.ROM - PHILIPSDISK.ROM 
* MSX2 Japanese : MSX2J.ROM - MSX2JEXT.ROM - MSX2PMUS.ROM - MOONSOUND.ROM - XBASIC2.ROM - PANASONICDISK.ROM - KANJI.ROM - MSXKANJI.ROM 
* MSX2 Korean : MSX2KR.ROM - MSX2KREXT.ROM - MSX2PMUS.ROM - MOONSOUND.ROM - XBASIC2.ROM - NATIONALDISK.ROM - HANGUL.ROM - MSX2HAN.ROM 
* MSX2 Only PSG : MSX2.ROM - MSX2EXT.ROM - XBASIC2.ROM - PHILIPSDISK.ROM 
* MSX2 Russian : MSX2R.ROM - MSX2REXT.ROM - MSX2PMUS.ROM - MOONSOUND.ROM - XBASIC2.ROM - NATIONALDISK.ROM 
* MSX2 Spanish : MSX2SP.ROM - MSX2SPEXT.ROM - MSX2PMUS.ROM - MOONSOUND.ROM - XBASIC2.ROM - PHILIPSDISK.ROM 
* MSX2+ : MSX2P.ROM - MSX2PEXT.ROM - MSX2PMUS.ROM - MOONSOUND.ROM - XBASIC2.ROM - PANASONICDISK.ROM - KANJI.ROM - MSXKANJI.ROM 
* Turbo-R : FSA1GT.ROM - KANJI.ROM - MOONSOUND.ROM - XBASIC2.ROM

If you're not sure about where to place your BIOS there is a Shared Roms folder you can also put them into (this only applies to ROMS that can be shared between different variants of MSX; Colecovision BIOS for example will not work if placed in the shared Roms folder.

```
/home/pi/RetroPie/BIOS/Machines/Shared Roms/
```

The following is a list of roms that can be added to the shared folder:


- ARAB1.ROM
- ARABIC.rom
- BEERIDE.ROM
- FMPAC.rom
- GCVMX80.ROM
- HANGUL.rom
- KANJI.rom
- MICROSOLDISK.ROM
- MOONSOUND.rom
- MSX2AREXT.ROM
- MSX2AR.ROM
- MSX2BREXT.rom
- MSX2BR.rom
- MSX2EXT.rom
- MSX2FREXT.rom
- MSX2FR.rom
- MSX2GEXT.rom
- MSX2G.rom
- MSX2HAN.rom
- MSX2JEXT.rom
- MSX2J.rom
- MSX2KREXT.rom
- MSX2KR.rom
- MSX2PEXT.rom
- MSX2PMUS.rom
- MSX2P.rom
- MSX2R2.ROM
- MSX2REXT.rom
- MSX2.rom
- MSX2R.rom
- MSX2SE.rom
- MSX2SPEXT.rom
- MSX2SP.rom
- MSXAR.ROM
- MSXBR.rom
- MSXDOS23.ROM
- MSXFR.rom
- MSXG.rom
- MSXHAN.rom
- MSXJ.rom
- MSXKANJI.rom
- MSXKR.rom
- MSXR2.rom
- MSX.rom
- MSXR.rom
- MSXSE.ROM
- MSXSP.rom
- MSXTREXT.ROM
- MSXTRMUS.ROM
- MSXTROPT.ROM
- MSXTR.ROM
- NATIONALDISK.rom
- NOVAXIS.rom
- PAINT.rom
- PANASONICDISK.rom
- PHILIPSDISK.rom
- RS232.ROM
- SUNRISEIDE.rom
- SWP.rom
- XBASIC2.rom

### Disc Swapping for Multi-disk Games in RetroArch (lr-blueMSX)

To change disks in-game, go to Core Disk Options > Disk Image Append.

### M3U playlist for Multi-disk Games

Multiple disks can be loaded simultaneously from Emulation Station into RetroArch by creating an M3U file (plain-text, ".m3u" extension). In it's contents, enter the filenames of the DSK files one per line. In game you can then swap disks from the core disk options menu (under Options). Make sure to cycle tray status before attempting to change disks.

## openMSX
openMSX will by default use a MSX2+ c-bios rom image. c-bios is not a real BIOS rom and has certain restrictions, such as no support for anything other then cartridges (ROMs). So there is no support for disk or cassette for instance.

You can change this by adding dumps of real MSX system roms into the ``/opt/retropie/emulators/openmsx/share/systemroms`` or the ``~/.openMSX/share/systemroms`` directory.

To locate real MSX system ROMs, try google.

### Changing default machine to be emulated
By default openMSX will emulate a MSX2+ using the c-bios ROMs. To change this, you need to start openMSX, either by starting a game or from the commandline by typing ``/opt/retropie/emulators/openmsx/bin/openmsx``

When the emulator is running, press `F10` and you will get a overlay where you can type commands, here you need to type the following to change the default MSX to be emulated;

``set default_emulator turbor``

In the above example we change the default to the MSX TurboR, which was the last MSX machine produced. Other options could be ``msx1``, ``msx2`` or ``msx2plus``. There are many MSX machines that can potentially be emulated, for a list look in the directory ``/opt/retropie/emulators/openmsx/share/machines``. If for instance you wanted to emulate a Spectravideo SVI-728 you will find in that directory a file ``Spectravideo_SVI-728.xml``, simply use the name of the file, excluding the .xml extension as the machine name.

Machine type msx1, msx2, msx2plus and turbor are simply links to certain MSX machines as follows;
- msx1 = European Toshiba HX10
- msx2 = European Philips NMS 8250
- msx2plus = Japanese Panasonic FS-A1WSX
- turbor = Japanese Panasonic FS-A1GT

The machine type selected will obviously have certain effects. For instance the FS-A1GT does not support cassettes, and so you cannot play cassette games on it. Also starting some games (mainly Konami) on a Japanese machine may result in the in-game dialogue being in Japanese, while if you start the same game on a European machine the in-game dialogue may be in English.

Note: If you do not have the ROMs for the default machine type requested in the correct location, openMSX will still start, but with the c-bios ROMs.

### Exiting the emulator
The key definitions defined in retropie will not work in openMSX. openMSX does however allow you to redefine your controls. For more information, look at the openMSX website for 'bind'.

By default the exit key in the emulator is ``Alt-F4``

### Setting default screen on MSX2+ and TurboR machines
By default MSX2+ and TurboR machines will start with a screen type which is incompatible with lots of European software. Typically resulting in errors such as ``Syntax error in 10`` when starting disk or cassette based games. This is typically because the software is trying to change the width of the screen to something incompatible with the current screen type selected. The solution is to start the emulator to a MSX BIOS Ok prompt. This can be done when a game fails to start and gives you an Ok prompt, or you can start the emulator outside of RetroPie as shown above.

At the MSX BIOS Ok prompt (not the openMSX command prompt), type the following;

``screen0``

``set screen``

You have now changed your default screen to screen0 as was normal on European MSX machines, and saved the setting into virtual nvram.

Note: if you change your default machine type from say a TurboR to a MSX2+ you will have to redo this step as each MSX2 and later machine type has its own virtual nvram file.

### 50 or 60Hz?
European MSX machines ran at 50Hz, as that is the PAL video standard. Japanese MSX machines however ran at 60Hz as is standard on NTSC. How does this effect things? Well it means that lots of Japanese developed games run ~20% slower when run on a European MSX. This may mean more sluggish behaviour and slower sound if the programmers did not take this into account.

How does this effect emulation? The default c-bios roms use 60Hz. If you use real MSX system roms, then it depends on which machine your emulating. A MSX2+ or TurboR will always be 60Hz since they where never officially sold in Europe.

Of course the effect can also be the other way around. European MSX software that runs too fast on a Japanese machine type.

In openMSX, you can change the emulated frequency during runtime. Simply open the openMSX command prompt with `F10`, and type `toggle_freq`.