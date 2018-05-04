# cap-electrodes
Capacitive Electrodes team for ECE 522 (Spring 2018)

### Scripts
- `AT.ino`:   for configuring HC-05 Bluetooth module via AT commands
- `rtbt.ino`: for operating the Arduino Uno and HC-05
- `bt_ecg.m`: for collecting data from the Arduino Uno and analyzing it

### Setup
- check the `rtbt.ino` for pin configurations of Arduino
- disconnect TX/RX
- upload `rtbt.ino`
- reconnect TX/RX
- run `bt_ecg.m`
