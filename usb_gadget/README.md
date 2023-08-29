# usb gadget module configuration for [rpizero-hid](https://github.com/Pant3x/rpizero-hid)

To be able to use `rpizero-hid` package
it's necessary to change some configuration on the kernel.

### Install / remove the module
clone the repo if you haven't yet
```bash
git clone https://github.com/Pant3x/rpizero-hid
```

get into usb_gadget folder
```bash
cd rpizero-hid/usb_gadget
```
give the installer permission and execute `installer.bash`
```bash
chmod +x installer.bash && sudo ./installer.bash
```
