# hideproc

這個專案是 2021 年暑期 Linux 核心課程的homework1

## Usage
```
$ sudo insmod hideproc.ko 
$ pidof cron
$ echo "add 644" | sudo tee /dev/hideproc 
$ pidof cron # 無法見到 cron
$ echo "del 644" | sudo tee /dev/hideproc 
$ pidof cron # 再次見到 cron
$ sudo rmmod hideproc
```