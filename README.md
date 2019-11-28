# Simple Serial Protocol
This protocol is designed for general purpose serial computer-to-machine communication (also machine-to-machine).
It should be simple, robust, based on low-bytes-data-transfer and most of all user friendly. 
On one side it has to perform well on low resource devices like microcontrollers.
On the other hand it needs to feel comfortable for Highlevel-Programming, powered by modern programming languages.
...
Let's close the gap.

## Kick off Platforms and Languages
* [Simple Serial Protocol for Arduino]
* [Simple Serial Protocol for Node.js]

## Shout out to Antonin Raffin
The Simple Serial Protocol is inspired by Antonin Raffin's minmalistic primitive datentypes approach.
The author has written an article at Medium.com [Simple and Robust Computer Arduino Serial Communication].

## Datatypes and Traffic Consumption
### Logic values
* **boolean**: true or false (8bit)
### Characters and Text - (printable ASCII only)
* **char**: single character (8bit/1byte)
* **text**: char array / c-string (variable data size)
    * single character (8bit/1byte)
    * plus end-of-string (8bit/1byte)(non-printable ASCII) 
### Numeric values
* **int**: integer value (16bit) 
    * signed -32,768 to 32,767
    * unsigned 0 to 65,523 
* **long**: (32bit) Große zahlen
    * signed -2,147,483,648 to 2,147,483,647
    * unsigned 0 to 4,294,967,295  
* **float**: (32bit)
    * ± 3.402,823,4 * 10^38

### Limitations
* Text/Characters only printable ASCII

## Links
[Simple Serial Protocol for Arduino]:https://gitlab.com/yesbotics/simple-serial-protocol/simple-serial-protocol-arduino
[Simple Serial Protocol for Node.js]:https://gitlab.com/yesbotics/simple-serial-protocol/simple-serial-protocol-node
[Simple and Robust Computer Arduino Serial Communication]:https://medium.com/@araffin/simple-and-robust-computer-arduino-serial-communication-f91b95596788
[araffin/arduino-robust-serial]:https://github.com/araffin/arduino-robust-serial
__