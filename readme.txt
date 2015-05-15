This is a modified I2C arduino library.  Derived from two-wire library from IDE version 1.6.2

You may replace the original "wire" library by renaming 
newWire.cpp and newWire.h to Wire.cpp and Wire.h and replacing the contents of the original
"wire" library. 

You may also use as a seperate library and wherever you would use #include<Wire.h>
just put #include<newWire.h> instead.

Differences from the default library:
	*Timeout to prevent I2C bus freezes 
	*Added configurable timeout value
	*Added better bus reset logic on a timeout
    *Changed default bus speed to 400KHz in twi.h
	*Added an internal pull-up function to enable or disable internal pull-ups