# Washer Notifier

> Source code accompanying the video at <https://www.youtube.com/watch?v=atD7VcXrfWY>

Leaving the clothes in the washer for too long? Need a way to detect when the washer is done?
In this video I walk you through the process I went through to create such a device and the
related automation code.

I build a little sensor using an ESP-01 and an accelerometer (MPU6050) that send off data to my
home assistant instance. The programming was done using [ESPHome](https://esphome.io/). A
[home assistant](https://www.home-assistant.io/) automation then takes these readings and detects
when the washer is complete and announces over Amazon Echo and Google Home devices in the home.

This is part 1 of the project. In this part I wrote a little [python script](http://bit.ly/36YOT1f)
to read the sensor readings from ESPHome and dump it into a CSV file. Using a
[Jupyter notebook](https://jupyter.org/),
I then load this CSV file and plot the sensor values. This made it easy to try out various
algorithms to identify the washer cycles.  I also explain (briefly) the process of writing custom
 code to convert this algorithm into a custom filter that acts on the sensor readings in ESPHome.

## Links:

* [Schematic](http://bit.ly/2rf4BGa)

### Aliexpress:
* [Female Micro USB Connector](http://s.click.aliexpress.com/e/CWPZ2ZrS)
* [Small Box](http://s.click.aliexpress.com/e/BXgpWTYM)
* [MPU6050](http://s.click.aliexpress.com/e/qs81hpFa)
* [ESP-01](http://s.click.aliexpress.com/e/5LVC1OKM)
* [ESP-01 Programmer](http://s.click.aliexpress.com/e/qNMsgQBm)
* [3.3V regulator](http://s.click.aliexpress.com/e/DyoqPbhW)
* [Veroboard](http://s.click.aliexpress.com/e/FnTQdduy)
