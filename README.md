# Raspberry Pi DHT22 Weather Station Python Flask Socketio  
A DHT Weather Station project using Python, Flask, Flask-SocketIO, and Bootstrap that displays real-time temperature and humidity sensor readings using your Raspberry Pi

## Prerequisites
Make sure to install the DHT22 driver on your Raspberry Pi using the Adafruit_circuitPython_dht library.   

## How To Run
Command to start website:
flask run --host=0.0.0.0

Command to start Qemu raspberry pi emulator:
qemu-system-arm -M versatilepb -cpu arm1176 -m 256 -drive "file=2024-11-19-raspios-bookworm-armhf-lite.img,if=none,index=0,media=disk,format=raw,id=disk0" -device "virtio-blk-pci,drive=disk0,disable-modern=on,disable-legacy=off" -net "user,hostfwd=tcp::5022-:22" -dtb qemu/versatile-pb-buster-5.4.51.dtb -kernel qemu/kernel-qemu-5.4.51-buster -append 'root=/dev/vda2 panic =1' -no-reboot


