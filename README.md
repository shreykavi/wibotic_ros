#Wibotic ROS Package

###Description:
This package uses ws4py in a python script to retrieve data from the wibotic websocket. 
The data recieved is in binary format and has to be manipulated to make usable. The data 
is then organized and pushed to the '/wibotic_websocket' rostopic. Functions have also been 
included to send read and write requests for specific parameters. For more details on 
parameters look at the WiBotic_Network_API.pdf doc.

###How to use:
1. Add this to a ros project.
2. run 'rosdep update'
3. run 'rosdep install --from-paths src --ignore-src --rosdistro=kinetic -y' Note: change kinetic to your distro
4. source devel/setup.bash
5. run "rosrun wibotic_ros wibotic.py" to start publishing socket data to rostopic.

###Checkout the test folder for:
- Wibotic.html: an html tool for basic websocket communication
- WiBotic_Network_API.pdf: doc for Wibotic websocket api
