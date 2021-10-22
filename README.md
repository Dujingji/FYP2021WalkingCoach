# FYP2021WalkingCoach

FYP 2021 SEM2 A Reinforcement Learning Robot As A Walking Coach

Project description:
 
This project aims at developing an adaptive robot to encourage physical activities of its user, namely walking for a certain distance. 

The main objective of this project is to develop an adaptive Human Robot interaction system for encouraging physical activities of its users using reinforcement learning. The robot in this project is designed as a walking coach. This robot is able to use the detected energy value, velocities and  orientation of the users to adjust its actions in order to maintain the user's energy and orientation at a reasonable level so that they can achieve a predefined walking goal. In particular, the robot is required to achieve the following goals with the assumptions(the detailed discussion with be in the assumption section):
●	Keep the user’s energy value in a range of 40% to 60% as much as possible and never under 10% or above 90%. 

●	Keep the orientation of the users in a range of 85o to 95o as much as possible and never under 45o or above 135o, which means  the heading of the user should facing forward direction

●	Encourage users to walk as fast as possible to complete a task. 

●	The users have different personality types that influence their energy dynamics and reactions to different robot actions, and the robot can choose the right actions to interact with different users. 

●	Social norms of personal and social space must be applied all the time during the task. 

FYP Presentation video YouTube link: https://youtu.be/BLkgsN60Rrg

FYP final version code:https://drive.google.com/file/d/1vHCN70daaB5ZPKDPt-nsmhYTI9JVdPpf/view?usp=sharing

FYP simulation video: https://drive.google.com/file/d/17HiVEIuDnhEmLfJH6Qejn1iI8yok0oSK/view?usp=sharing

FYP code execute guide video: https://drive.google.com/file/d/1wsemLcGq_shd40U_wuByctbX-osxrNdZ/view?usp=sharing

Addition guild video for testing: https://drive.google.com/file/d/1SGOJfn4y_OFEkilh-FjkjX0Maq0HzHR9/view?usp=sharing










The code and information of the project 
Here is the project code and animation video and execution guide video

You can run the code followed by the video guide. 

Remember to initialize ray but rar.init() and uncomment or comment the line in the Social norm Class depends on your testing or training. 

The final report is submitted in the moodle 

The animation description is here: 
The animation can be found in the link . The simulation shows how the human and robot interact in the 2D environment. The human agent will first initial a random energy, orientation and personal type. The robot will be 3.6m right behind the human agent as it’s the Social range of the social distance, Then the robot will take an action from action space. The energy and the orientation will change based on the action. Then the robot will base on the energy of the human to move to the desired personal range(learn from the SoicalNorm network). The assumption here is, when the human has higher energy, the robot will more likely move to personal space or stay in the social space. When the human has low energy, the robot will move to social space or public space. Meanwhile, the robot will never enter the intimate space. The reason why I make this assumption is, when a person has more energy, usually a human is more acceptable to a robot to be closer to them. Otherwise, the human will feel uncomfortable with a robot close to them. And the robot should never move to the intimate range as it’s very dangerous. 
The simulation is simultaneous and both robot and agent update in the same step !.  




The checkpoint_ 000030 is for the myENV class
The checkpoint_ 000010 is for the SoicalNorm class




