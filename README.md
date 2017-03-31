# WebClubController

Apache Module to Control an RLC Club Controller via Serial Port

https://www.rlccontrollers.com/store/p1/RLC-Club_Controller.html


Development will be started with the assumption that we're going to use 9600, N, 8, 1 for serial port interation on a Linux Apache 2.4 installation with serial port /dev/ttyS0 (COM1)

I'll just create the module so it's flexible and take an authentication token and numeric command.

The web interface I can build later and have that do the authentication by whatever means necessary, then just hand back an authentication token which will get handed off to this module along with the command.

I am going to also assume www-data (or whatever account) will have access to the serial port - of course I'll have to do some error checking on that.
