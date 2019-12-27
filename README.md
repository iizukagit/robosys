# robosys
LEDを点灯させるデバイスドライバを作成しました。
デモ動画は https://www.youtube.com/watch?v=z1LEITZjFU4&feature=youtu.be です。

# dependency
使用言語はC言語です。

# Setup
$ make
$ sudo insmod myled.ko
$ sudo chmod 666 /dev/myled0 

# Usage
/dev/myled0に1を書き込むとLEDが光り0を書き込むとLEDが消灯します。
点灯：$ echo 1 > /dev/myled0
消灯：$ echo ０ > /dev/myled0

# References
https://ryuichiueda.github.io/robosys2019/lesson7.html#/32
