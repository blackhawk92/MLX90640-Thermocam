# MLX90640-Thermocam for Odroid GO


The German radio show Netzbasteln built a simple Thermal camera using the MLX90640 Sensor, an ESP32, a ILI9341 TFT, a 18650 battery in a 3D printed case. 
It was featured in Netzbasteln #111: http://www.netzbasteln.de/#111 and still lacks interpolation.

I rewrote some things to make it work on an Odroid Go and with the standard ESP32 core.

Code Based on:
- Thermal Camera with image saving capability https://github.com/wilhelmzeuschner/arduino_thermal_camera_with_sd_and_img_processing
- SparkFun MLX90640 Examples https://github.com/sparkfun/SparkFun_MLX90640_Arduino_Example
- TFT_eSPI Library: https://github.com/Bodmer/ (use settings from Setup_User.h)
- Alternative Wire code for standard ESP32 core https://github.com/sparkfun/SparkFun_MLX90640_Arduino_Example/issues/2#issuecomment-460422443

Hardware:
- Odroid Go: https://wiki.odroid.com/odroid_go/odroid_go
- MLX90640 Sensor Breakout Board: https://shop.pimoroni.com/products/mlx90640-thermal-camera-breakout (or the Sparkfun one)


Odroid Go Header Pins
```
GND 1
SENSOR_SDA 4
SENSOR_SCL 5 
VCC 6 
```
