# HM10-spin
-----------

This is a P8X32A/Propeller, ~~P2X8C4M64P/Propeller 2~~ driver object for HM10 Bluetooth-LE modules.

**IMPORTANT**: This software is meant to be used with the [spin-standard-library](https://github.com/avsa242/spin-standard-library) (P8X32A) ~~or [p2-spin-standard-library](https://github.com/avsa242/p2-spin-standard-library) (P2X8C4M64P)~~. Please install the applicable library first before attempting to use this code, otherwise you will be missing several files required to build the project.

## Salient Features

* UART connection at 9600bps
* Change module name
* Read module's MAC address
* Read module's firmware version
* Read last connected device's MAC address
* Set advertising interval
* Integration with lib.terminal.spin, for full terminal I/O support (Char(), Bin(), Dec(), Hex(), printf(), etc)

## Requirements

P1/SPIN1:
* spin-standard-library

~~P2/SPIN2:~~
* ~~p2-spin-standard-library~~

## Compiler Compatibility

* P1/SPIN1: OpenSpin (tested with 1.00.81)
* ~~P2/SPIN2: FlexSpin (tested with 5.3.0-beta)~~ _(not yet implemented)_
* ~~BST~~ (incompatible - no preprocessor)
* ~~Propeller Tool~~ (incompatible - no preprocessor)
* ~~PNut~~ (incompatible - no preprocessor)

## Limitations

* Very early in development - may malfunction, or outright fail to build
* Supports slave role only
* Only supports 9600bps connection

## TODO

- [ ] Port to P2/SPIN2
- [ ] Add support for other bitrates
- [ ] Add support for master role
- [ ] TBD