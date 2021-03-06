# Summary
The problem statement we have chosen is **Integrating with a Smart Environment**.  
Our solution aims to leverage on this interconnected network of devices within Singapore to enable a more timely response to emergency incidents. We believe that minimal delay and early intervention is key to prevent potential escalation of the emergency which can result in significantly greater damage to both infrastructure and human life. Additionally, minimizing  any potential obstacles on the road enable emergency vehicles a safer environment as the drivers will now be more aware of their presence.
&nbsp;  
## Situational Analysis
For our solution, we have a specific audience in mind. Drivers. That being said, there is a very limited number of available mediums to send a message due to the dangers of distraction while driving.
* Sound? They are in an enclosed area, possibly with a radio blasting in the back ground. Inefficient and won't be heard until its too late.  
* Digital? They're not supposed to check their phones.     
## [Solution?](solution/description.md)   
The only way through which drivers know to communicate. Visual cues.
* Want to change lane --> blinker lights
* Going to reverse --> back lights
* Somebody cut you off --> wave your hand angrily and hope they see your displeasure  
 
We chose to leverage on street lights and traffic lights as first and foremost, it is gives a clear and identifiable signal to the drivers. Different coloured street lights are clearly noticeable as it will definitely be an unusual sight on the road. And it is illegal to run a red light so drivers have to stop for the Emergency Vehicle.  
&nbsp; 
## Key Issues and Solution
The problem we identified is the accessibility of emergency vehicles (EVs) on roads facing heavy flow, leading to a delayed response time for EVs. Our solution incorporates existing infrastructure in order to compel drivers on the road to give way to approaching EVs.     
&nbsp;   
One **problem of the current solution (sirens)** is that by the time drivers are able to hear and locate the EV, it is already too near them and it would be too late to take prompt action. Thus, we need a method to signal drivers that they should clear a path before the EVs are too near, translating into less obstruction faced en route to their destination. In addition, the sound of sirens give some notion of where the Emergency Vehicle is coming from but far from clear indication.  
&nbsp;  
**Our solution** is to utilize street lights along Singapore’s roads by changing their colour to signal that emergency vehicles will be travelling on that road and they should start changing to the side lanes. Additionally, we will take control of the traffic lights en route to the emergency to enable a smoother journey.  
To put it simply, if the street lights on your road flashes red, an emergency vehicle is coming from behind.  
**Move to the side.**   
&nbsp;     
When an EV is dispatched to a location, the most direct route can be calculated, and lights along the roads to the destination within an estimated 5min travel time will change colour. This change of colour signals to drivers that they should clear the way for oncoming EVs. 


# Strategy and Recommendations
A key feature of our solution is that it provides a direct benefit to the SCDF once implemented. It will be able to quicken their response time significantly, especially during peak hours.  
This quicker response time can translate to many other tangible benefits. 
* Earlier intervention enables the situation to be better controlled and can save precious resources which might have been required to deal with a more extreme case.  
* Minimal damage to infrastructure and human life. The earlier the responders reach, the quicker they can deal with any situation, the faster it can be resolved.   
&nbsp;  
&nbsp;   

Alternatively, our solution provides a safer work environment for these emergency responders. 
* On the road, traffic lights are changed in their favour so no more running of red lights.
* Drivers are alerted of the incoming presence of emergency vehicles. No more unwary changing of lanes.
* At the scene of the emergency, the street lights can further serve as visual cues to stay away from the area as there is an emergency.

&nbsp;  
&nbsp;   
In order to realize our solution, the Node-RED on the IBM Cloud platform is an excellent choice to control and manage our devices. A cloud environment also makes possible greater edge computing capabilities without the need for corresponding hardware at the street lights and traffic lights.
&nbsp;  
&nbsp;   
In our [humble prototype](solution/description.md), we demonstrate the utilization of node-red to send signals to "street lights" to alter their behaviour.

# Project Roadmap
This details the various steps to be taken from the development of software infrastructure to deployment. It is a step by step process to enable each functionality before combining it into our final solution.
1. Develop capability to control lights via cloud. 
1. Develop software to predict and anticipate the best route, and detect all the relevant lights along the route
1. Integrate location of Emergency Vehicle for real time update of best route and relevant lights. (might change route based on driver)
1. Test sync of information to send real time commands to IoT devices.
1. Pilot in a built environment

&nbsp;  
&nbsp; 

# Implementation
## Plan of action
1. Develop and test solution
1. Start deployment and pilot on existing built environments.
1. After successful pilot, expand implementation as Singapore moves towards a smart nation.

## Challenges
1. There is a lot of resources required, software and hardware development and deployment, before the solution can reach a level feasible for tangible results
1. Requires widespread implementation of Internet of Things (IoT) devices.
    1. Can be worked around by systematically installing IoT capabilities on street lights whenever they are due for maintenance.
1. Requires drivers to be educated on the significance of street lights changing colours.  
1. Requires long-term education in civic-mindedness and road signals, which can be incorporated into the Theory Tests in driving schools so that future generations of drivers will be more aware.

&nbsp;  
&nbsp; 

# Conclusion
> "Time is of the essence"    

We hope to shorten response time and get the responders to where they need to be, quickly and safely.  
There is much existing infrastructure currently available for us to tap upon. In this case, the rows and rows of streetlights that serve no other purpose than lighting our roads at night.  
The only thing stopping our emergency responders from action is the time it takes to get to the scene, and delays on the road is one thing that we can definitely minimize. 
This first step however, could be that small push to bring about a large distributed information network that the SCDF can rely on to gather information and prepare for beforehand.  
An emergency? Trigger the nearby nodes to get information of the situation. 
* Where exactly is the incident? 
* How many people are there? 
* What are the environmental conditions? 
#### To sum it up,
The integration Internet of Things enable us to make **_our roads smarter, our city safer, our first responders more efficient._**
