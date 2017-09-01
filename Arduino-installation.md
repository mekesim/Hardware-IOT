# 安装Arduino编辑器

1. 到[Arduino官网](/www.arduino.cc)下载安装最新版本的编辑器\(IDE\)。  
   可以使用它编程和下载程序到Arduino板。也可以使用官网提供的在线[编辑器](https://create.arduino.cc/editor)，不过需要安装插件。

2. 安装打开编辑器，连接开发板到电脑。

3. 选择合适的端口。一般会自动选择，如果有多个设备连接到电脑手动选择合适的端口。  
   ![](/assets/import.png)

## Wemos 安装

### Installing the CH340G Drivers

CH340G is a cheap serial to USB programming chip and does not come with native windows or mac drivers. However it has been made very easy to install.

Download and install the drivers [here](https://github.com/mekesim/Hardware-IOT/blob/master/assets/CH341SER.zip).

After instanllation, connect USB cable to PC, it will find there is a USB-SERIAL CH340 item under Ports \(COM & LPT\).

![](/assets/comport.png)

### Test Wemos

* Start Arduino and open Preferences window.
* Enter http://arduino.esp8266.com/stable/package\_esp8266com\_index.json into Additional Board Manager URLs field. You can add multiple URLs, separating them with commas.
* Open Boards Manager from Tools &gt; Board menu and find esp8266 platform.
* Select the version you need from a drop-down box.
* Click install button.
* Don't forget to select your ESP8266 board from Tools &gt; Board menu after installation.

You may optionally use staging boards manager package link: http://arduino.esp8266.com/staging/package\_esp8266com\_index.json. This may contain some new features, but at the same time, some things might be broken.



