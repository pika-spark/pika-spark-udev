<a href="https://pika-spark.io/"><img align="right" src="logo/logo-pika-spark-bg-white.png" width="15%"></a>
:sparkles: `pika-spark-udev`
============================
[![Spell Check status](https://github.com/pika-spark/pika-spark-udev/actions/workflows/spell-check.yml/badge.svg)](https://github.com/pika-spark/pika-spark-udev/actions/workflows/spell-check.yml)

Setting the right [udev](https://en.wikipedia.org/wiki/Udev)-rule allows flashing of the Arduino Portenta X8 on [Pika Spark](https://pika-spark.io/) without requiring super-user (`root`) privileges.

<p align="center">
  <a href="https://pika-spark.io/"><img src="https://raw.githubusercontent.com/pika-spark/.github/main/logo/logo-pika-spark-bg-white-github.png" width="40%"></a>
</p>

### How-to-`udev`
```bash
https://github.com/pika-spark/pika-spark-udev
sudo cp pika-spark-udev/99-uuu.rules /etc/udev/rules.d/
sudo udevadm control --reload-rules
sudo udevadm trigger
```

For further information on how to flash the Arduino Portenta X8 please refer to the official [documentation](https://docs.pika-spark.io/flash/).
