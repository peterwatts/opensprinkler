=======================
=== !!!IMPORTANT!!! ===
=======================

*DO NOT* download .hex files directly from GitHub page by using 'Save File As...' or 'Save Link As...'. Instead, download the entire package as a zip file, or alternatively download individual files using the 'Raw' link.

***************************************
***************************************
This firmware is for hardware 2.1 only.
It will NOT work on other versions.
***************************************
***************************************

=== Update since 2.0.2 ===
- Fixed a bug that can lead to incorrect running time when NTP sync takes too long (longer than a station's water time).
- Provided an option to change Javascript url. The default path is http://rayshobby.net/scripts/java/svc2.0.3. To change it, use
  http://x.x.x.x/su
  where x.x.x.x is your OpenSprinkler's IP address.
  To host the Javascript locally on the uSD card, follow the instructions below to prepare the uSD card, and then change the Javascript url to
  .
  (i.e. dot)
- Added support for MCP7940N RTC (pin compatible with DS1307)
===========================

This firmware (2.0.3) provides an option to make use of a microSD card to store and serve Javascripts required for rendering OpenSprinkler webpages. This is NOT required. To use this feature, please read the instructions below:

* A microSD (uSD) card of 2.0 GB or below (NOTE: cards with more than 2.0 GB capacity are not supported)
  Here is an inexpensive uSD card that comes with an adapter and makes it easy to copy file in the next step:
  http://www.amazon.com/gp/offer-listing/B000PC62O6/
  
* Copy all the files in the 'copy_to_sd' folder to your uSD card's root directory. 
  It's important that these files are in the root directory, not in a subdirectory!
  
* Flash the new firmware, by following the README.txt in the folder one level above.
  =======================
  === !!!IMPORTANT!!! ===
  =======================
  - Flashing a new firmware to your OpenSprinkler will erase all settings and program data.
    Make sure you record or back up your settings and data before re-flashing.

* Once the controller starts, if the uSD card is detected successfully, you will see an SD card
  icon displayed at the right end of the LCD screen. It looks like this:
  ┌────┐
  ├────┤
  │   ┌┘
  └───┘  If you don't see this icon, check to make sure your uSD card is inserted securely.
