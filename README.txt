== DCS-BIOS

DCS-BIOS is a community-maintained `Export.lua` file for use with DCS: World.
It provides a stable, documented interface for external hardware and software to interact with the clickable cockpit of a DCS: World aircraft.

  Info: Since the Website was down, every information is included in the Repositorie here.
  Also we add the arduino-library and com-handler to save it, so they don't get lost. 
  But we can't maintain them.

== For Panel Builders

You don't need to be a programmer or electrical engineer.
The DCS-BIOS User Guide will show you step by step how to connect your panel to DCS using DCS-BIOS and the beginner-friendly Arduino microcontroller platform.
You don't have to write any program code yourself.

== For Software Developers

The Developer Guide explains how to connect to and interpret the DCS-BIOS export data stream and how to send commands to DCS-BIOS to operate controls inside the cockpit.

== Is My Aircraft Supported?

Currently, DCS-BIOS supports the following aircraft modules:

* A-4E-C (contributed by Dehuman){ get the Mod here: https://forums.eagle.ru/showthread.php?p=3930571}
* A-10C (FSF-Ian)
* AJS-37 (contributed by pdmarsh extended by BlackLibrary,ArturDCS)
* AV8BNA (contributed by BlackLibrary)
* Bf-109-K-4 (contributed by ArturDCS)
* C-101CC / EB (contributed by BlackLibrary,cdpkobra) (use C-101CC for All Versions)
* Christen Eagle II (contributed by BlackLibrary,cdpkobra)
* F-14B (contributed by BlackLibrary,ArturDCS)
* F-5E-3 (contributed by geebeer2, extended by BlackLibrary)
* F-86F (contributed by ArturDCS)
* F/A-18C (contributed by AndrewW)
* FC3 (contributed by danvac, extended by BlackLibrary)
* FW-190-A8 (contributed by BlackLibrary,MD44)
* FW-190-D9 (contributed by ArturDCS)
* I-16 (contributed by BlackLibrary,NightStalker)
* Ka-50 (contributed by airtom)
* L-39ZA / C (contributed by kadda11, overhauled by BlackLibrary) (use L-39ZA for All Versions)
* M-2000C (contributed by Exo7,ArturDCS)
* MB-339PAN (contributed by BlackLibrary){ get the Mod here: http://www.freccetricolorivirtuali.net/mod%20ftv.htm}
* Mi-8 (contributed by ArturDCS)
* MiG-15bis (contributed by BlackLibrary,Steve Gee)
* MiG-21Bis (contributed by wraith444)
* NS430 (contributed by Capt_Zeen, extended by Imp, revised by Celemourn)
* P-51D (contributed by pdmarsh)
* Spitfire
* SA 342 (all Versions) (use SA342M for All Versions)
* TF-51D (contributed by pdmarsh, ArturDCS)
* UH-1H (FSF-Ian)
* Yak-52 (contributed by BlackLibrary,cdpkobra)
* Externals for all Airplanes (Speedbrake and Lights)
* All Flaming Cliffs 3 Modules (FC3) (A-10A;F-15C;J-11A;MiG-29A;
  MiG-29S;Su-25;Su-25T;Su-27;Su-33)
* Mods (FC3): VSN-Mods, PAK-FA Project, Civil Aircraft Mod, Upuaut's Bell-47G, Mirage F.1, SU-30 FAMILY PROJECT, MIG-23UB Project,
              Virtual Cockpits, AC-130
  
  Use always the latest version of the Mods!
  
  For DCS Flightpanels: 
  FC3 are only supported with Keyemulator. But some Exports can made as Strings (FC3.lua) and CommonData 

If you want to add support for another module, please get in touch.

== Mod Support

If you want to add a FC3 based Mod (eg. VSN_Mod Planes) for commondata suport, you must follow
these instructions:

Add at the bottom  in \DCS-BIOS\lib\AircraftList.lua

a("PlaneName", false)

To get the correct Plane Name, open the control-reference page while you fly that plane. 
In MetadataStat you find the Plane Name.

== For setting up the Control-reference Page:

1. Install Google Chrome
2. Chrome -> "Settings" -> "More Tools" -> "Extensions", check "Developer mode"
3. Click "Load unpacked extension..." and choose your "C:\Users\<username>\Saved Games\DCS\Scripts\DCS-BIOS\doc" folder
4. A new extension "DCS-BIOS Control Reference Live Preview" 
   will be visible under "Apps".
5. Exit "Settings"
6. Start DCS, load a Mission and jump in a Plane
7. Click "Apps" in your Browser. Your DCS-BIOS extension be there. From there you can see the controls change as you fly and manipulate the cockpit. 

  Remember to refresh the page if you restart a mission, so Chrome gets a new connection to DCS-BIOS.

== socat

There are 2 socat vesions, 32 and 64 bit. Choose that version that fits best for you. 
The files in the zip File must be unzipped direct in the socat folder.

  The path must be: /socat/socat.exe

== Video Tutorials

https://www.youtube.com/channel/UCwECFPfC3QJiNYS5fskF2vg/

== Contribute

If you have a question or found a bug, please open an issue on the GitHub issue tracker.
https://github.com/dcs-bios/dcs-bios/issues/new

If you want to contribute code or documentation, please send a pull request on GitHub.

== License

The orginal DCS-BIOS was programmed by [FSF]Ian. This is a Fork of his Repositorie, where we made some additions and changes to it.

DCS-BIOS is released under a slightly modified Simple Public License 2.0 (think "a version of the GPL readable by mere mortals"). Please see `DCS-BIOS-License.txt`.

The copy of `socat` that comes with DCS-BIOS is licensed under the GPLv2 (see `socat/COPYING`).

== Support

* We have a Discord: https://discord.gg/5svGwKX
* https://github.com/DCSFlightpanels/DCSFlightpanels
* https://github.com/DCSFlightpanels/DCS-Flightpanels-Profiles
* If you want to support us: https://www.paypal.me/jerkerdahlblom
