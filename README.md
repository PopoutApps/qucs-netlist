# qucs-netlist

This version v0.1.0 is for Linux.

Converts Qucs-s schematic files into a netlist file suitable for Veroboard/stripboard PCB design applications, currently only DIY Layout Creator. If there is also a Qucs-s .sim file with the same name but the .sim extension, it will use that to create the nets, if not it will attempt to run Qucs-s to create a .sim file. If no .sim file was present and can't be created, the output netlist file will contain components but no nets.

**Simplest Installation** Download the qucs-netlist executable. 

Copy it somewhere convenient. 

To run it, click on the blue diamond icon. 

(To remove it just delete it.)

**Integrated Installation** If you want it on the desktop menu, or are reluctant to trust the executable. 

Download the qucs-netlist.tar.gz file. 

Double-click it to extract it to a directory called qucs-netlist. 

Double-click the directory to open it, you should see: 

install.sh

qucs-netlist

qucs-netlist.dat

qucs-netlist.desktop

qucs-netlist.hlp

qucs-netlist.png

qucs-netlist.py

uninstall.sh

Right click on install.sh then select Run as a Program.

Enter your password.

You can delete the qucs-netlist.tar.gz and the qucs-netlist directory after installation, but keep uninstall.sh.

(Run uninstall.sh in the same way as you ran install.sh to remove it.)

To run it, find the icon on the Gnome menu and click on it.

**Running it**

Choose the schematic file you want, it will output a file with the same name in the same directory, but with the extension .net. Eg example.sch will produce example.net. It will also produce an intermediate file called example.sim which can be deleted.

There will be a message with a warning line for each component which is not yet in the reference data file, for example:

Warning: Unknown component type not converted: D2 Diac

I can add components to the data file if requested.

The exported file can be imported by DIY Layout Creator (available from their website), but I could adapt it for others Stripboard software if requested.

There is a maximum of 1000 components.

