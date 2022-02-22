# Seeed_reTerminal_Bridge_RS232_exmaple

![](https://files.seeedstudio.com/wiki/reTerminal_Bridge/reTerminal_bridge.jpg)
 
Example Python code for using RS232 on reTerminal Bridge.

Since the RS485 function uses ttyS0, it is necessary to close the ttyS0 system interaction function before starting.

```sh
$ sudo raspi-config
```

Select **Interface Options**, **Serial port** in turn. 
On the next screen you will be prompted if you want to login shell accessible over serial, select **No**. 
Then in “Do you want to use serial port hardware”, make sure **Yes** is selected with. 
After reTerminal has made changes, you will see the following text appear on the screen. 

Use a cable to connect the reTerminal Bridge to the computer via the RS232 interface.

One of the reTerminals compiles and runs the code that sends the data.

```sh
$ sudo python3 rs232_send.py
```

Another reTerminal compiles and runs the code that receives the data.
```sh
$ sudo python3 rs232_receive.py
```

## Getting Started

- [reTerminal Bridge wiki]()

