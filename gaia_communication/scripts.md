---- Para utilizar a library serial:

```bash
$ pip install pyserial
```

Setup Serial:

```bash
$ sudo raspi-config
```

Selecione interfacing options -> Serial -> Yes e Yes to reboot 

---- Para utilizar a library gpsd:

```bash
$ sudo apt-get install gpsd-clients gpsd -y
```

** Se você estiver usando gpsd manualmente, você precisa iniciá-lo antes de rodar gpsmon ou cgps:

```bash
$ sudo gpsd /dev/ttyS0 -F /var/run/gpsd.sock
```

Para testar:

```bash
$ sudo cgps
```

Após isso:

```bash
$ sudo killall gpsd
```

