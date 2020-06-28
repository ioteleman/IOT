![result](https://github.com/ioteleman/IOT/blob/master/final-prj/high.jpg)

iot final project  

1-Setting up a wireless LAN via the command line in rpi  

2- VNC (Virtual Network Computing)  

3- MQTT Libraries  
To use MQTT with the ESP8266 we’ll use the Async MQTT Client Library.  

4- Installing the ESPAsync TCP Library  

To use MQTT with the ESP, you also need the ESPAsync TCP library.  

5- install MQTT Mosquitto Client:  

`pi@raspberry:~ $ sudo apt-get install mosquitto-clients`  

6- Installing Node-RED  
Getting Node-RED installed in your Raspberry Pi is quick and easy. It just takes a few commands.  

Having an SSH connection established with your Raspberry Pi, enter the following commands to install Node-RED:  

`pi@raspberry:~ $ bash <(curl -sL https://raw.githubusercontent.com/node-red/raspbian-deb-package/master/resources/update-nodejs-and-nodered)`  
The installation should be completed after a couple of minutes.  

7- Autostart Node-RED on boot  
To automatically run Node-RED when the Pi boots up, you need to enter the following command:  

`pi@raspberry:~ $ sudo systemctl enable nodered.service`  
Now, restart your Pi so the autostart takes effect:  

`pi@raspberry:~ $ sudo reboot`  
Testing the Installation  
When your Pi is back on, you can test the installation by entering the IP address of your Pi in a web browser followed by the 1880 port number:  

http://YOUR_RPi_IP_ADDRESS:1880  

8- Autostart mosquitto on boot  

`pi@raspberry:~ $ sudo systemctl enable mosquitto.service`  

9- Installing Node-RED Dashboard  
To install the Node-RED Dashboard run the following commands:  

`pi@raspberry:~ $ node-red-stop`  
`pi@raspberry:~ $ cd ~/.node-red`  
`pi@raspberry:~/.node-red $ npm install node-red-dashboard`  
Then, reboot your Pi to ensure that all changes take effect on Node-RED software:  

`pi@raspberry:~ $ sudo reboot`  
To open the Node-RED UI, type your Raspberry Pi IP address in a web browser followed by :1880/ui as shown below:  

http://Your_RPi_IP_address:1880/ui  

10- for installing led in node-red ui use this command:

npm install node-red-contrib-ui-led  
