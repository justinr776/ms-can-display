The OLED displays can be damaged if they are repeatedly powered off without being placed in a safe state by software.

The method used on this project is to provide sufficient bulk capacitance for the display to sense the supply drop and perform the required shut down routine before the input voltage drops too low.

http://www.tincannetwork.com/files/AutoShutdown1.PNG

The second IO pin is used to check if the display is shut down before power drops.

http://www.tincannetwork.com/files/AutoShutdown2.PNG

For more details see the display source code.