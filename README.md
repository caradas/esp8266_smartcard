# esp8266_smartcard

Use esp8266's GPIO to simulate a smart card,
while running an oscam client,
connecting to the cccam server via esp8266's wifi.

So as to achieve the set-top box DVB CW sharing.


English (machine translation) below
使用esp8266来模拟智能卡，把esp8266接到标准的机顶盒读卡器上，从而实现cccam共享。
要用到四根数据线连接读卡器和esp8266的gpio端口。
分别是vcc、gnd、5、2。
gpio 2 为io，连接到到读卡器io
gpio 5 为rst，连接到到读卡器rst。

在某些情况下，需要在esp8266的io和rst到读卡器间，要串联一个470欧的电阻。



本项目用arduino打开编译，需要安装esp8266支持库和ESPAsyncTCP库。
目前支持了永新同方卡的模拟。长时间观看会出现不稳定现象，原因未知。
想折腾的可以添加其它卡支持。

Use esp8266 to simulate a smart card, and connect esp8266 to a standard set-top box card reader to realize cccam sharing.
Four data cables are needed to connect the card reader and the gpio port of the esp8266.
They are vcc, gnd, 5, and 2.
gpio 2 is io, connected to the card reader io
gpio 5 is rst, connected to the card reader rst.

In some cases, a 470 ohm resistor needs to be connected in series between the io and rst of the esp8266 and the reader.



This project is opened and compiled with arduino, and esp8266 support library and ESPAsyncTCP library need to be installed.
Currently supports the simulation of Yongxin Tongfang Card. Long-term viewing will cause instability, the reason is unknown.
If you want to toss, you can add other card support
