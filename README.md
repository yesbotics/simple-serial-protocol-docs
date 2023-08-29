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

### Byte values
* **byte**: integer value (8 bit / 1 byte)

### Logic values
* **boolean**: true or false (8 bit / 1 byte)

### Characters and Text - (printable ASCII only)
* **char**: single character (8 bit / 1 byte)
* **text / string**: char array / c-string (variable data size)
    * single character (8 bit / 1 byte)
    * plus end-of-string (8 bit / 1 byte) (non-printable ASCII char `\0`) 

### Numeric values
* **tiny integer**: (8 bit / 1 byte) 
    * signed -128 to 127
    * unsigned 0 to 255 
* **small integer**: (16 bit / 2 bytes) 
    * signed -32,768 to 32,767
    * unsigned 0 to 65,523 
* **integer**: (32 bit / 4 bytes)
    * signed -2,147,483,648 to 2,147,483,647
    * unsigned 0 to 4,294,967,295  
* **big integer**: (64 bit / 8 bytes)
    * signed -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807
    * unsigned 0 to 18,446,744,073,709,551,615
* **float**: floating point values (32 bit / 4 bytes)
    * -3.402,823,4 * 10^38 to 3.402,823,4 * 10^38

### Limitations
* Text/Characters only printable ASCII

## Shout out to Antonin Raffin
The Simple Serial Protocol is inspired by Antonin Raffin's minimalistic primitive datatypes approach.
The author has written an article at Medium.com [Simple and Robust Computer Arduino Serial Communication].

## Links
[Simple Serial Protocol for Arduino]:https://github.com/yesbotics/simple-serial-protocol-arduino
[Simple Serial Protocol for Node.js]:https://github.com/yesbotics/simple-serial-protocol-node
[Simple Serial Protocol for C++]:https://github.com/yesbotics/simple-serial-protocol-cpp
[Simple and Robust Computer Arduino Serial Communication]:https://medium.com/@araffin/simple-and-robust-computer-arduino-serial-communication-f91b95596788
[araffin/arduino-robust-serial]:https://github.com/araffin/arduino-robust-serial
__
