# Summary
The problem statement we have chosen is **Integrating with a Smart Environment**.  
Our solution aims to leverage on this interconnected network of devices within Singapore to enable a more timely response to emergency incidents. We believe that minimal delay and early intervention is key to prevent potential escalation of the emergency which can result in significantly greater damage to both infrastructure and human life. Additionally, minimizing  any potential obstacles on the road enable emergency vehicles a safer environment as the drivers will now be more aware of their presence.
&nbsp;  
## Key Issues and Solution
The problem we identified is the accessibility of emergency vehicles (EVs) on roads facing heavy flow, leading to a delayed response time for EVs. Our solution incorporates existing infrastructure in order to compel drivers on the road to give way to approaching EVs.
&nbsp;   
One problem of the current solution (sirens) is that by the time drivers are able to hear and locate the EV, it is already too near them and it would be too late to take prompt action. Thus, we need a method to signal drivers that they should clear a path before the EVs are too near, translating into less obstruction faced en route to their destination.
&nbsp;   
Our solution is to utilize street lights along Singapore’s roads by changing their colour to signal that emergency vehicles will be travelling on the road and they should start changing to the side lanes. Additionally, we will take control of the traffic lights en route to the emergency to enable a smoother journey. 
&nbsp;   
When an EV is dispatched to a location, the most direct route can be calculated, and lights along the roads to the destination within an estimated 5min travel time will change colour. This change of colour signals to drivers that they should clear the way for oncoming EVs. 

# Strategy and Recommendations
A key feature of our solution is that it provides a direct benefit to the SCDF once implemented. It will be able to quicken their response time significantly, especially during peak hours.  
This quicker response time can translate to many other tangible benefits. 
* Earlier intervention enables the situation to be better controlled and can save precious resources which might have been required to deal with a more extreme case.  
* Minimal damage to infrastructure and human life. The earlier the responders reach, the quicker they can deal with any situation, the faster it can be resolved.

Alternatively, our solution provides a safer work environment for these emergency responders. 
* On the road, traffic lights are changed in their favour so no more running of red lights.
* Drivers are alerted of the incoming presence of emergency vehicles. No more unwary changing of lanes.
* At the scene of the emergency, the street lights can further serve as visual cues to stay away from the area as there is an emergency.

&nbsp; 
In order to realize our solution, the Node-RED on the IBM Cloud platform is an excellent choice to control and manage our devices. A cloud environment also makes possible greater edge computing capabilities without the need for corresponding hardware at the street lights and traffic lights.
In our humble prototype, we demonstrate the utilization of node-red to send signals to "street lights" to alter their behaviour.

# Implementation and Plan of Action

