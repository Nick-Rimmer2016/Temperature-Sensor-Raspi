## Hot Tub Temperature Sensor   


Add the following to config.txt   - ```dtoverlay=w1-gpio,gpiopin=17,pullup=on```    
Add the following to /etc/modules - ```w1-therm strong_pullup=1```   
Run ```sudo modprobe w1_therm```   
Run ```sudo modprobe w1_gpio```   

Check sensor   
cd /sys/bus/w1/devices   

Reference:   
https://www.circuitbasics.com/raspberry-pi-ds18b20-temperature-sensor-tutorial/#:~:text=The%20DS18B20%20temperature%20sensor%20is,accurate%20and%20take%20measurements%20quickly.   

### Install Apache   

```sudo apt-get update```   
```sudo apt-get upgrade```   

```sudo apt install apache2 -y```   

sudo usermod -a -G www-data pi   
sudo chown -R -f www-data:www-data /var/www/html   

sudo nano /var/www/html/index.html   

Remember certificate for https   
Ref: https://pimylifeup.com/raspberry-pi-apache/