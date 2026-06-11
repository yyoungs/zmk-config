1. List the USB devices attached, you should see cradio/demeter or something

```
lsusb
```

1. Enter bootloader mode.
1. List usb devises again. You should see nice!nano
1. Create a tmp dir

```
mkdir -p /tmp/nicenano/
```

1. Mount the board
```
sudo mount -o rw /dev/sda /tmp/nicenano
```
1. Copy over the firmware
```
sudo cp ~/Downloads/firmware/demeter_right-nice_nano_v2-zmk.uf2 /tmp/nicenano/
```
1. Continue to ls the dir until it becomes empty
```
ls /tmp/nicenano/
```
1. Unmount the drive
```
sudo umount /tmp/nicenano
```
1. unplug the board.
