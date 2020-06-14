# How does it work?
## Well, here's our thought process:
1. First, there is an emergency alert somewhere (simulated in this case)
1. A software computes the shortest route from the emergency vehicle to the location and identifies all the relevant lights.
1. Node-RED sends signals to these lights to turnn them on.

## So what does our prototype say?
Our prototype aims to visualize the possibility to do remote control of the lights through Node-RED using the IBM cloud. Albeit a manual process at the moment, we hope to show that a simple click of a button (or rather, eventually the trigger of a software) will be able to send signals to the lights to behave accordingly.  
  
## Scalability potential
Having our Node-RED process connected to the IBM cloud enables us to do any necessary computations without the corresponding hardware constraint at the edge. Additionally, a cloud network facilities information gathering where we we can further scale our solution to include sensors and collect data at the scene of the emergency. 
  
For instance. Say there was a fire, we could gather information like:
* **Noise levels**: Are there many people screaming? That could indicate the severity of the situation.
* **Is it raining?**: That certainly changes the environment and we should prepare beforehand.
* **Motion detection**: Are there a lot of people at the area? 
* **Object detection**: With a distributed network (each with a camera) connected to the cloud, compute is less of an issue and we can leverage on this to even identify the exact location of the emergency before we even reach the scene.

Simply identify and activate the nodes at the scene, and we will be able to obtain a comprehensive map of the environmental conditions.

## Physical Prototype
### Display of our flows on Node-RED
![node-red flows](images/node_red_flows.jpeg?raw=true "Node-RED Flows")
Trigger --> hardware control
### Node-RED interface for the prototype
![node-red interface](images/light_config_on.jpeg?raw=true "Node-RED Config")
A manual trigger (automated eventually) sends a signal to the hardware device to change the light display.
### Top view of Arduino board
![top-view arduino](images/arduino_top_view.jpeg?raw=true "Arduino Top View")  

### All lights off
![all lights off](images/lights_off.jpeg?raw=true "Lights off Arduino")  
No lights are on when all settings are set to "off" state  

### Selective lights on  
![all lights on](images/lights_on.jpeg?raw=true "Lights on Arduino")
Lights are turned on based on settings given in Node-RED  

# Getting Started
## Set-up
### Arduino
1. Open the StandardFirmata.ino file on Arduino IDE. 
  * StandardFirmata.ino is available in the Arduino IDE by default. (File -> Examples -> Firmata -> StandardFirmata)
  * Alternatively, it can be accessed via this link: [https://github.com/firmata/arduino#firmata-client-libraries](https://github.com/firmata/arduino#firmata-client-libraries)
1. Wire up the circuit as shown in the [top-view diagram above](###top-view-of-arduino-board)
  * We use digital pins 2, 7 and 8 in this example. Each pin is used to control the 'Street Lamps' (LEDs) of a particular 'Lane' (circuit).
1. Compile and upload the StandardFirmata.ino file into the Arduino

### Node-RED
1. Open the Node-RED Editor
1. Import the flows.json file
1. Go to the dashboard and control the street lamps!

## Running Tests
Connect up the arduino and check if clicking the buttons on the dashboard in Node-RED causes the LEDs to light up.

## Live Demo
<video width="320" height="240" controls>
  <source src="images/arduino_demo.mp4" type="video/mp4">
</video>

## What did we use?
* Node-RED deployed on IBM cloud.
* Arduino as a simulated micro-controller.
(A Raspberry Pi would have been a better choice to show online connection to the cloud but unfortunately we did not have any on hand)
