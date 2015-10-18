# Serial.print() extension with Xterm codes #

Arduino Serial.print() lacks capability to output information in structured way.
By using Xterm control sequences it's possible to easy follow changes in debug variables.

Download library, install it as required for your OS. There is example file.

Example usage
```
xterm.print(1,1,"This is normal text",NORMAL); 
            | |  |                    |
            | |  |                    +- display atribute
            | |  +- text or variable
            | +- row
            |
            +- column
```


On Mac OSX use iTerm (http://iterm.sourceforge.net/) and initiate session with

```
screen /dev/name_of_your_arduino_port 
```


On Windows use free PuTTY (http://www.chiark.greenend.org.uk/~sgtatham/putty/)