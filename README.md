# DPS201: Lab PSU
DPS201 is a software controlled lab power supply designed for hobbyists and students. It features a single output channel which is programmable from 0V to 20V in 100mV steps. It also sports a current limiting feature which can be programmed from 0A to 1A in 10mA steps. 

**This repo** holds the hardware design files for the DPS201, you can find the firmware repo [here](https://github.com/mannsi/PS201) and the accompanying software repo [here](https://github.com/mannsi/PsController). Both the firmware and software are still under developement. A complete project page, with updates and more, can be found on [hackaday.io](http://hackaday.io/project/1948)

## gEDA source files
The entire project is designed using the open source software bundle [gEDA](http://www.geda-project.org/). 
### Schematic
In order to view the schematic you must run the command
```
$ gschem DPS201_schematic.sch
```
from within the repo. `gschem` then loads the accompanying configuration file: `gschemrc`. This file makes sure that all symbols needed are loaded from the `SYMBOLS` directory.
### Layout
The PCB layout can be accessed using the `pcb` software that comes with `gEDA`. Simply run
```
$ pcb DPS201_layout.pcb
```
from the terminal.

## pdf and Gerbers
In the repo you can also find pdf file for the schematic, and gerber files in the directory `GERBERS`. These should be enough to manufacture a DPS201 pcb and assemble with the help of the component mapping image: `DPS201_component_mapping.jpg`.

## Assembly
All components can be ordered from Digikey, Farnell or other distributers. The assembly can be carried out by hand with some care, note that most resistors and caps are 0603 and the IC's have small pin pitch. Nevertheless, one can solder all the components on the board by hand.
