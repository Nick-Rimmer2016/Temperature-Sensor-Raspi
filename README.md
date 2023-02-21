## Temperature Sensor for my Hot Tub

Add the following to config.txt   - ```dtoverlay=w1-gpio,gpiopin=17,pullup=on```    
Add the following to /etc/modules - ```w1-therm strong_pullup=1```   
Run ```sudo modprobe w1_therm```   
Run ```sudo modprobe w1_gpio```   

Check sensor   
cd /sys/bus/w1/devices   


https://www.circuitbasics.com/raspberry-pi-ds18b20-temperature-sensor-tutorial/#:~:text=The%20DS18B20%20temperature%20sensor%20is,accurate%20and%20take%20measurements%20quickly.