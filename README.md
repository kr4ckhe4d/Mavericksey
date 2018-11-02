Mavericksey
===============

A script for OS X to display system information

!['Screenshot'](http://i.imgur.com/ftUfa1Z.png)


Install / Uninstall
------------
Use 'install.sh` to both install and uninstall.

Add the following line at the end of your ~/.bash_profile:

    mavericksey
    
or this one to have colored logo:

    mavericksey -c
    
or this one to have colored logo and a customized welcome message name:

    mavericksey -c -n "John Doe"


Options
------------
	-n,  --name
		Set custom name for welcome message.
	-c,  --color
		Color Logo
		
	-red
		Red Text
		
	-green
		Green Text
	
	-yellow
		Yellow Text
		
	-blue
		Blue Text
		
	-purple
		Purple Text
		
	-grey
		Grey Text

Recent Changes
--------------

* (Addtion) Options for changing text color
* (Optimization) Removed Escape Characters from ASCII art
* (Optimization) Renamed color variables to all be same length - helps when echoing
* (Optimzation) Aligned ASCII art / text in echo statement
* (Addition) Added model field to display Mac Model ID


To-Do List
------------

Bug Fixes / Optimization
* Test Package Manager with macports
* Look into $terminalText bug. Maybe find a better way of displaying colors then current method
* Code cleanup
* Update Screenshots
* Fix uptime alignment bug
* Better way of changing text color (use ""-text blue"" or "-text red" rather then "-red" or "-blue")

Features
* Smarter install script (create directory if doesn't exist, prompt if already uninstalled)
* Look into being able to install via package manager (homebrew / macports)
* Display more precise model details (e.g. iMac 27-inch, Late 2012)
* Display Graphics Card Model (system_profiler SPDisplaysDataType)
* Display Total Hard Drive Space on Disk (currently shows only a percentage)
