.. ESPprogrammer Docs documentation master file, created by
   sphinx-quickstart on Thu Jun 18 19:00:23 2020.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

ESP Programmer
=========================================

.. image:: images/espprogrammerallhookedup.png
   :align: center

.. raw:: html

    <div style="text-align: center; margin-bottom: 2em;">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/41L3wW0PhGo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>

**What is it?** 
----------------

* Standalone ESP32 board to easily upload bin files to a target ESP32.  Great for factory programming or just updating firmware in existing systems without a need for OTA or connecting to a computer.  No messing around with IDE's or Command line! 
* Uploads bin files from included 8GB micro SD card. These are the same exact bin files that are uploaded when you click "upload" from the Arduino IDE.
* Powered by micro USB power or 4.2V lithium battery (built in charger), which makes the board versatile for updating boards in the field.  
* Target board is programmed from standard UART connection and also toggles DTR/RTS line, to activate auto-reset circuit for ESP32 to enter download mode. 
* Simple two button interface for mass programming START and RESET
* On board jumper selects power output from JST PH 2.0mm connector.  3.0V is a controlled power source, which is useful for integrating a power cycle from the programmer as well as for calibration.  Other selections that are always on, 5V, 3.3V, and the raw Battery voltage. 
* 1x6 female connector for "FTDI" style cables, and 2x3 IDC male header, which is nice for Tag Connect Cables
* EXPANSION!  All spare IO broken out to pads, which could be used to control an automated fixture - relays, sensors, etc... or even if the auto-reset circuit requires RTS and CTS signal.  
* It's based on an ESP32!  This means you have the ability to activate an AP for your target ESP32 to connect to and communicate with.  The trigBoard tester firmware did just this and sent over messages containing critical board information that was part of the automated test sequence.  You also have bluetooth available as well. 
* The board provides a 6 pin UART interface that can be used to provide information back up to a PC.  Test logs, MAC address, etc... Even had one customer consider using this with a thermal printer. 

**Where to buy?**

.. raw:: html

   <div>
   <a href="https://www.tindie.com/stores/kdcircuits/?ref=offsite_badges&utm_source=sellers_kdcircuits&utm_medium=badges&utm_campaign=badge_large"><img src="https://d2ss6ovg47m0r5.cloudfront.net/badges/tindie-larges.png" alt="I sell on Tindie" width="200" height="104"></a>
   </div>

For higher quantities or OEM opportunities, please `contact KD Circuits directly <https://www.kdcircuits.com#contact>`_

.. toctree::
   :maxdepth: 2 
   :caption: ESPprogrammer Docs

   usage.rst
   source.rst










