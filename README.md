

HID python library for emulating mouse and keyboard on PI zero.

## Setup - Tested on [Raspbian](https://www.raspberrypi.com/software/operating-systems/#raspberry-pi-os-32-bit) lite 5.10

1. Install apt dependencies

```bash
sudo apt-get update
sudo apt-get install -y git python3-pip
```  


2. install usb gadget module  https://github.com/Pant3x/rpizerohid/tree/main/usb_gadget
3. Install `rpizerohid` with `pip`
```bash
pip3 install rpizerohid
```

## Usage
Note: You should connect the data usb port (left one) to the raspberry, and NOT the power port  
  
- Control mouse
```python
from rpizerohid import Mouse
m = Mouse()
for i in range(5):
    m.move_relative(10, 10)
```
- Control keyboard
```python
from rpizerohid import Keyboard

k = Keyboard()
k.type('Hello world!')
```
