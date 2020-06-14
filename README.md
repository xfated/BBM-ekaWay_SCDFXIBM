# BBM  
_Here to make a difference._  
&nbsp;    
&nbsp;  


# INTEGRATING WITH A SMART ENVIRONMENT
--------------------------------------------------------------------------------------------------------------------------------  
## Problem Statement 
Infrastructure is getting “smart”, with sensors and Internet of things (IoT) increasingly embedded in the built environment (e.g. Punggol Digital District). How might we leverage a network of smart
infrastructure in the built environment to make better and more timely sense of emergency
incidents (e.g. detection of fires developing, building collapses, falls, road traffic accidents etc.) and
to trigger early intervention measures, without the need to activate precious emergency resources?
  
&nbsp;  
## What's the problem and why is our solution better.
Today, there is no strict protocol for drivers to adhere to when they see an emergency vehicle on the road. At best, the drivers simply slowly move towards the side of lanes once they see an emergency vehicle in their rear view mirror. But too often, by the time they hear or see an emergency vehicle on the road, it is likely that it is too late for them to react and the road conditions might not be favourable for them to move out of the way.   
Additionally, the lack of a well-followed procedure results in the [lack of regard](https://www.straitstimes.com/forum/letters-in-print/motorists-continue-to-impede-emergency-vehicles) towards a sense of urgency when making way for emergency responders.  
Let us note one of the [existing protocols](https://www.todayonline.com/singapore/more-emergency-vehicles-allowed-beat-red-lights-faster-response-scdf) for drivers of emergency vehicles whose priority is rushing to a scene of emergency:
> “When approaching a traffic junction, the driver must also slow down and come to a complete stop so that an assessment of the traffic situation can be made before proceeding further.”  

We feel that there is an **unnecessary delay** that can be **removed by leveraging on a connected network of Internet-of-Things devices** to **preemptively clear the road for emergencies**.

Local example:
<p align="center">
  <img src="ambulance_delay.jpg?raw=true" alt="Ambulance Delayed" width=60%>
</p>
<p align="center">
Photo Credits: the new paper <br />
<a href="https://www.tnp.sg/news/others/ambulance-rushing-woman-hospital-blocked-pie-heartless-road-hog-causes-deadly-delay"> Ambulance rushing woman to hospital blocked on PIE: Heartless road hog causes deadly delay </a>
</p>  
   
&nbsp;   

   
## Our solution.
#### how?
Our solution aims to **notify drivers in advance** and **make the journey smoother and more efficient** for the emergency vehicles  
* Using the streetlights as visual signals for drivers to keep to the side of the roads
* Preemptive control of traffic lights to prepare an uninterrupted route to the scene of an emergency.

#### why?
* Drivers will now know beforehand that emergency vehicles are approaching and they have ample time to clear to the sides.
* Emergency vehicle drivers can better focus on getting to the destination when the roads are clear and traffic conditions all in their favour.

&nbsp;  
Ideal Situation:  
<p align="center">
  <img src="road_halt_for_ev.jpg?raw=true" alt="Road clears for emergency vehicle") width=50%/>
</p>  

<p align="center">  
Photo Credits: <a href="https://www.reddit.com/r/Damnthatsinteresting/comments/99c65h/when_traffic_comes_to_a_complete_stop_in_germany/">Reddit</a>
</p>  


# [An Overview of our solution](detailed_desc.md)
1. Emergency alert raised from a source.
1. SCDF activated
1. Software generates the shortest path from SCDF branch to the scene.
1. Location of the Emergency Vehicle continually uploaded to the cloud.
1. Based on location of Emergency Vehicle, identify all relevant street lights and traffic lights (on route and within a defined radius)
1. Send signals via cloud to turn street lights red, traffic lights to change in favour of the emergency vehicle’s route.
1. After the Emergency Vehicle passes the location, release control of the lights.

&nbsp;  


# Solution Implementation
_As our desired spans a rather large scale, we have developed a small prototype to illustrate what our ideal solution aims to achieve_ that is detailed [here](/solution/description.md).
