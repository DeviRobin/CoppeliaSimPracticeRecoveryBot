Real-time search-and-rescue robots are increasingly used to supplement the efforts of the first responders in areas affected by natural disasters. They are used to spot-check the situational awareness of people in distress, survey the extent of flood or tornado damage, evaluate the number of people that had not been evacuated from their neighborhoods, clean debris, and create passable routes.
For this task, you will use the Coppelia Robotics virtual robot and its environment to demonstrate how such robots may be used in disaster recovery. Your first step is to familiarize yourself with this technology by reviewing the information in the “Coppelia Robotics Resources Page” and “CoppeliaSim User Manual” provided in the Web Links section.
For the next step, you will thoroughly describe a disaster situation similar to the ones mentioned above. Next, you will create a virtual prototype of an autonomous robotic recovery system that demonstrates goal-seeking behaviors in navigating through a predefined area. The robotic recovery system will solve a disaster recovery problem of your choice by using the Coppelia Robotics BubbleRob and its environment as the starting point of your prototyping. You will also add sensors to the robot. These sensors will collect vital information to aid in the disaster recovery effort for the scenario you described.

A.  Describe the disaster recovery environment you chose and the two obstacles you have added to the environment. 
•	This disaster environment emulates a house after tornado damage. The obstacles in this room include two fallen racks, a fallen dining chair and an electrical fire. These are all likely obstacles present at the scene of homes following a disaster such as a tornado. 

B.  Explain how the robot will improve disaster recovery in the environment from part A after you have added the two obstacles from part A. 
•	This upgraded robot will improve disaster recovery in this environment by providing a method of scouting disaster areas prior to sending in rescue workers. This robot can provide rescue workers with information regarding the layout and situation in the room prior to their entry. This robot is also small enough to manuver through the bostacles such as the fallen racks and chairs unlike rescue workers who will have to physically move all obstacles prior to entry. 

C.  Justify the modifications you made to CoppeliaSim’s robot architecture, including two sensors you chose to add, and explain how these sensors will aid the disaster recovery effort. 
•	Two significant modifications to the CoppeliaSim’s BubbleRob include two additional sensors in addition to the proximity sensor. The first sensor is a proximity sensor that identifies people in the room. This sensor will turn from green to blue in the case of a fire and report ‘person detected’. This will aid disaster recovery by alerting rescuers of a person's existence in rooms and rubble before they have to enter. This will prevent needless risk by ensuring rooms without people are passed over during disaster recovery. The second sensor is a proximity sensor that can identify fires in the room. This sensor will turn from white to red in the case of a fire and report ‘fire detected’. This sensor provides vital information to rescue workers and can be used to ascertain whether fire rescue equipment will be needed on-site. These two sensors are vital for discovering situations where immediate rescue is needed due to the presence of fire in the room as well as a fallen person. 

D.  Describe how the robot maintains an internal representation of the environment. 
•	The robot maintains an internal representation of the environment using a proximity sensor that detects objects at a range of .30 meters away. This allows the robot to detect obstacles from a distance and perform evasive techniques to avoid colliding with the environment. The robot also has additional sensors to detect fire and people. These can help alert the bot and users to important environmental factors that must be addressed by rescuers. 


E.  Explain how the robot implements the following four concepts to achieve its goal: 

•	reasoning 
    The robot implements reasoning by using the data it collects via its various proximity sensors to respond to the environment. When an obstacle is detected, the robot decides to turn to avoid it. 

•	knowledge representation 
    The robot implements knowledge representation by using the environmental information gained via its sensors to make decisions and reports. The proximity sensor helps the robot map out the path it will take to avoid obstacles in its path. Also, the fire and person detection allows the robot to report the presence of these elements in its environment. 

•	uncertainty 
    The robot implements uncertainty when it needs to decide on a path despite lacking a complete map of its environment. At times, proximity sensor readings are uncertain due to noise from partially blocked paths or lighting conditions. Currently uncertainty is responded to with caution, and the robot attempts to map a path of avoidance around obstacles even if they are possible false negatives. 

•	intelligence 
    The robot implements intelligence by moving autonomously though the disaster environment. It processes sensor data constantly and creates a path to avoid obstacles. 


F.  Explain how the prototype could be further improved, including how reinforced learning and advanced search algorithms can improve the prototype’s performance and learning. 
•	This prototype can be further improved by implementing a mapping and memory system that logs the coordinates of obstacles as they are encountered. It can also be improved by ensuring the robot does not get too close to a location when fire is detected. This can be done by using reinforced learning and advanced search algorithms. By implementing a penalty whenever a fire is approached and a reward when a person is approached, the robot can learn to maintain its distance from the fire and search for people. One specific example is implementing Q-learning, allowing the robot to map sensory input to its actions and learn more effective methods for navigating disaster locations. The robot can also use algorithms such as Dijkstra’s to calculate the best routes around obstacles to objectives. Overall, using both RL and advanced search algorithms can make the robot more adaptive and functional in the dangerous environments it will be required to operate in. 


G.  Submit the robot code that you created. 

•	Please see the attached .ttt file 
•	 This is the original code from CopelliaSim Edu BubbleRob Robot. 

