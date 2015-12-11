1. Install the Ardunio IDE. Windows installer available here: http://www.arduino.cc/en/Main/Software

2. If your board has an 8Mhz crystal then you need to take the core files here:

http://www.tincannetwork.com/files/at90can.zip

If your board has a 16Mhz crystal then you need the core files from here:

http://85.12.32.240/~superkoe/arduino/at90can.zip

http://www.tincannetwork.com/files/8Mhz.JPG

3. Extract the core files into your Arduino IDE folder such that you have the following:

![http://www.tincannetwork.com/files/SettingUpTheCore.png](http://www.tincannetwork.com/files/SettingUpTheCore.png)

4. Add the Metro library to your Arduino libraries directory. Available from here:

http://www.arduino.cc/playground/Code/Metro

5. Start the IDE and open the latest code. The main file to open is: "ms-can-display\Supported\AT90CAN128AT90CAN128.pde"

![http://www.tincannetwork.com/files/IDE1.png](http://www.tincannetwork.com/files/IDE1.png)

6. To program the board a TTL RS232 connection is required. Here is an example with "programmer" used for the 4DGL displays. It is really just an FTDI USB to serial adaptor.

![http://www.tincannetwork.com/files/ProgrammerConnections.png](http://www.tincannetwork.com/files/ProgrammerConnections.png)

7. Select AT90CAN128 as the development board.

![http://www.tincannetwork.com/files/IDE3.png](http://www.tincannetwork.com/files/IDE3.png)

8. Hit "Verify" to generate a .Hex file for programming. Assuming the code compiled with no errors:

9. Remove the connector for the ribbon cable to the OLED display.

10. Power off the board.

11. Hit "Program"

![http://www.tincannetwork.com/files/IDE2.png](http://www.tincannetwork.com/files/IDE2.png)

12. When you see "Binary sketch size: ...." re-apply power to the board. You have to be quick!

![http://www.tincannetwork.com/files/Nowturnonpower.png](http://www.tincannetwork.com/files/Nowturnonpower.png)

The code should now be downloaded to the board.