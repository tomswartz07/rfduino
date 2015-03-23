# RFduino

A suite of Arduino sketches and libraries to transmit and receive data via [Amplitude Shift Keying](https://en.wikipedia.org/wiki/Amplitude-shift_keying) and Manchester encoding.

The code contained in this repository is specifically tailored to a set of 315MHz RF hardware.

If you dislike the Arduino IDE, there is a Makefile provided to help quickly build and upload the sketches.
The Makefile has been tested for use with the latest versions of Arduino and avrdude.

## Quick Start

Hook up an Arduino via USB.  
Double-check the Makefile and verify the settings are correct for your setup.

Move the appropriate sketch out of the `files` directory into the root.
Edit the Makefile `PROJECT` variable to reflect the name of the .ino file.

```bash
$ make
$ make upload
```

## Acknowledgments
Much of the Manchester Encoding logic and headers were adapted from [mchr3k/arduino-libs-manchester](https://github.com/mchr3k/arduino-libs-manchester).
