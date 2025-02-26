# Reading Data of GY-91 Sensor using I2C communication


## Code structure
- Read I2c address from GY-91 sensor using `i2c address check.txt`
- Read gyro data from gy-91 in degrees/sec using `gyro_read_gy_91.txt`

## Connections for I2C Communication
GY-91 -> ESP32
VCC          -> 3.3V
GND          -> GND
SCL          -> GPIO22
SDA          -> GPIO21

## Running the Code
- In arduino
	- change the file `i2c address check.txt` to `<name-here>.ino`
	- import the file into `ArduinoIDE` and upload it to ESP32
	- get the data from `Serial Monitor`
	- don't forget to set the `Baud rate` according to the code to display the data in correct form in serial monitor.
- In PlatformIO/VS code
	- change `<name-here>.txt` to `main.cpp`
	- move `main.cpp` into `src` folder of platformIO project
	- build it and upload the code to esp32
	- get the data from `Serial Monitor`
	- don't forget to set the `Baud rate` according to the code to display the data in correct form in serial monitor.
	
## References
- [Carbon aeronautics](https://github.com/CarbonAeronautics?tab=repositories)
