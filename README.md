# qucs-netlist

This version v0.1.0 is for Linux.

Converts Qucs-s schematic files into a netlist file suitable for Veroboard/stripboard PCB design applications, currently only DIY Layout Creator. If there is also a Qucs-s .sim file with the same name but the .sim extension, it will use that to create the nets, if not it will attempt to run Qucs-s to create a .sim file. If no .sim file was present and can't be created, the output netlist file will contain components but no nets.

**Linux**

**Simplest Installation**
  Download the qucs-netlist executable.
  Copy it somewhere convenient.
  To run it, click on the blue diamond icon.
  (To remove it just delete it.)
    
**Neatest Installation** If you want it on the desktop menu, or are reluctant to trust the executable.
  Download the qucs-netlist.tar.gz file.
  Copy it somewhere convenient.
  Extract it to get:
    qucs-netlist.desktop
    qucs-netlist.dat
    qucs-netlist.hlp
    qucs-netlist.py
    qucs-netlist.png
    qucs-netlist
    install.sh
    uninstall.sh

  Open a terminal, go into that directory, type ./install.sh.
  You can delete the qucs-netlist.tar.gz and that directory after installation, but keep uninstall.sh. 
  To run it, find the icon with the Gnome menu and click on it.
  (Run uninstall.sh to remove it.)

**Running it**
  Choose the schematic file you want, it will then output a file with the same name, but the extension .net. Eg example.sch will produce example.net. It will also produce an intermediate file called example.sim which can be deleted.

  There will be a message with a warning line for each component which is not yet in the reference data file, for example: Warning: Unknown component type not converted: D2 Diac

  I can add components to the data file if requested.

  The exported file can be imported by DIY Layout Creator (available from their website), but I could adapt it for others Stripboard software if requested.
  
    There is a maximum of 1000 components.
