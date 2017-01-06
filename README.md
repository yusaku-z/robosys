# myled.c
LED点灯のデバイスドライバ

# bashファイル
flash.bash 0.5秒の間隔で30回点滅する

# 配線
Raspberry piの22番ピン(GPIO25)にLEDを配線

# 使用方法
$ make
$ sudo insmod myled.ko
$ sudo chmod 666 /dev/myled0
$ sudo ./flash.bash
$ sudo rmmod myled
$ make clean

# 動画
https://www.youtube.com/watch?v=ve6Y1f4-xr0
