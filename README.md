Instructions to Reinstall and Rerun the app in case an os reset is required 

firstly install the rasbian 64 bit debian based os ( 2.4gb ) and copy it to the sd card using the pi imager 

Insert the newly written card to the memory card slot ,  connect the camera , keyboard mouse and hdmi cable 


Power on the raspberry pi by connecting it directly to the charger to avoid low voltage warnings ( use a 2 amps charger with fast charging capable cable ) ,

connect the other end of hdmi to usb streaimg device , now connect it to your laptop usb port

Now your raspberry pi's hdmi out will be recognised as a webcam source , you can use any camera apps as the display , just select the input source as Usb A or Usb B, set the resolution as required , 1080 X 720 , worked best for my device 

now you should be able to stream your pi's display
 
enable ssh and picamera , ctrl+alt+t opens the terminal , run command sudo raspi-config , this will open the connection settings , from interfacing options enable legacy camera , come back save the changes and exit , now reboot the system when prompted 

, check if the camera is working , run the command    raspistill -o test.jpg , this should take a picture , if not you have to reconfigure 

then clone this repository using the command       git clone  https://github.com/jagannath-p-s/pifinal.git 

navigate inside the folder , run pip install flask , pip install hx711 , 
