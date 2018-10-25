# rpi-clock
Simple Raspberry Pi clock using two Max7219 8x8 dot matrix display

To run:
1. buy this display unit (or similar) : https://www.ebay.ca/itm/Raspberry-Pi-LED-Display-Matrix-MAX7219-Dot-Matrix-Module-for-RPi-Model-B-B-/281644858680?hash=item4193577d38

2. download the .c file
3. install bcm2835 library: https://www.airspayce.com/mikem/bcm2835/
4. run the following command:

```
gcc -o timeDisplay timeDisplay.c -lbcm2835
sudo ./timeDisplay
```

Note: `sudo` is required because you need access to the SPI interface
