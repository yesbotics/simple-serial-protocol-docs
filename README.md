# Simple Serial Protocol
This protocol is designed for general purpose serial computer-to-machine or machine-to-machine communication.
It should be simple, robust, based on low-bytes-data-transfer and most of all user friendly. 
On one side it has to perform well on low resource devices like microcontrollers.
On the other hand it needs to feel comfortable for Highlevel-Programming, powered by modern programming languages.

Let's close the gap!

## Supported Platforms and Languages
* [Simple Serial Protocol for Arduino]
* [Simple Serial Protocol for Node.js]

## Datatypes and Traffic Consumption

### Logic values
* **boolean**: true or false (8 bit / 1 byte)

### Byte value
* **byte**: integer value (8 bit / 1 byte)

### Characters and Text - (printable ASCII only)
* **char**: single character (8 bit / 1 byte)
* **text**: char array / c-string (variable data size)
    * single character (8 bit / 1 byte)
    * plus end-of-string (8 bit / 1 byte) (non-printable ASCII char `\0`) 

### Numeric values
* **int**: integer value (16 bit / 2 bytes) 
    * signed -32,768 to 32,767
    * unsigned 0 to 65,523 
* **long**: big integer values (32 bit / 4 bytes)
    * signed -2,147,483,648 to 2,147,483,647
    * unsigned 0 to 4,294,967,295  
* **float**: floating point values (32 bit / 4 bytes)
    * ± 3.402,823,4 * 10^38

### Limitations
* Text/Characters only printable ASCII

## Shout out to Antonin Raffin
The Simple Serial Protocol is inspired by Antonin Raffin's minimalistic primitive datatypes approach.
The author has written an article at Medium.com [Simple and Robust Computer Arduino Serial Communication].

## Links
[Simple Serial Protocol for Arduino]:https://gitlab.com/yesbotics/simple-serial-protocol/simple-serial-protocol-arduino
[Simple Serial Protocol for Node.js]:https://gitlab.com/yesbotics/simple-serial-protocol/simple-serial-protocol-node
[Simple and Robust Computer Arduino Serial Communication]:https://medium.com/@araffin/simple-and-robust-computer-arduino-serial-communication-f91b95596788
[araffin/arduino-robust-serial]:https://github.com/araffin/arduino-robust-serial
__