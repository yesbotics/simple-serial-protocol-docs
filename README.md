# Simple Serial Protocol Documentation

## Beschreibung des Umfangs bzw. Ziels dieses Protokolls
* general purpose - define ur own ssp-based protocol
* event-based (callbacks)
* low bytes data transfer (based on fundamental c/c++ datatypes)
* robust (low memory-safe)

## Platformen / Sprachen
* [Simple Serial Protocol for Arduino]
* [Simple Serial Protocol for Node.Js]

## Protokoll Dokumentation

### Inspired by Antonin Raffin's minmalistic primitive datentypes approach
* read Medium.com article [Simple and Robust Computer Arduino Serial Communication](simple-and-robust-computer-arduino-serial-communication)
* git repo [araffin/arduino-robust-serial](https://github.com/araffin/arduino-robust-serial)

### Datentypen und Bereiche

* bool (8bit)

* char (8bit) Einzelne Zeichen
    * signed -128 to 127
    * unsigned 0 to 255

* int or short (16bit) (short kann raus oder?)
    * signed -32,768 to 32,767
    * unsigned 0 to 65,523 

* long (32bit)
    * signed -2,147,483,648 to 2,147,483,647
    * unsigned 0 to 4,294,967,295
    
* float (32bit)
    * ± 3.402,823,4 * 10^38

* string (variable länge)
    * pro ascii einzelzeichen 8bit
    * plus 8bit für end-of-string

## Links
[Simple Serial Protocol for Arduino]:https://gitlab.com/yesbotics/simple-serial-protocol/simple-serial-protocol-arduino
[Simple Serial Protocol for Node.Js]:https://gitlab.com/yesbotics/simple-serial-protocol/simple-serial-protocol-node
[Simple and Robust Computer Arduino Serial Communication]:https://medium.com/@araffin/simple-and-robust-computer-arduino-serial-communication-f91b95596788

