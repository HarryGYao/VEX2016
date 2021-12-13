# VEX 2016: Nothing But Net
![VEX2016](/images/Game.png)  
This is my source code for VEX Robot Championship in 2016. You can find the game there :[Nothing But Net](https://www.roboticseducation.org/vrc-nothing-but-net/).  
Also, you can find my team there: [7627A](https://www.robotevents.com/teams/VRC/7627A), I am serving as the main programmer in VRC 2015-2016: Nothing But Net (Yes, the best score in the team history!).  
Written in *easyC V4 for Cortex*. They are providing [V6](https://shop.intelitek.com/easyC-V6-for-IQEDR--Perpetual_p_122.html) now, check it out.
## About the Robot  
![OurRobot](/images/TheRobot.jpg)  
Our robot is a catapult with one extra shooting device: a firing pin to handling the long-range shooting.
## The Basic Structure
Since this is my first "meaningful" program, it contains a lot of *BAD* habit. 
**Please forgive me naming the variable by pinyin, commenting by Chinese, and even using the unmeaningful word "hhh", I was young :P**  
The main() contains three functions: Initialize(), Autonomouse() and OperatorControl().
## Initialize():  
Initialize() did **NOTHING**. Yes, I do not know what is Initialize at the time I write this program, so I left it blank.
## Autonomouse():  
In the Autonomous stage, the robot operated **ONLY** by this function, with no player control.  
It basically does two things: the firing pin shoots the preloaded balls and moves to the center of the game field.
## OperatorControl():
Here is the play control stage, since it's a catapult, I write a special function for loading the ball.  
zidonglaxixan(): means automatic pull the rubber band to providing the force of shooting.  
The robot has two sensors for detecting the loading stage.
It is working like this:
1. Checking if the robot is already for loading. If so, start loading balls and waiting for the play to shoot.
2. If not, stoping the loading function, or the robot will be useless.
3. Then the robot starts to lock the loading plane, or the loading plane will rise when we try to pull the rubber band. (Remember it is a catapult). One sensor will let the robot know the loading plane is locked.
4. After locking, the motor pulls the rubber band to the perfect length by time (data collected by my own experiment :P), and stop the motor when it has done(Told by another sensor).
5. Finally, the robot is ready for loading!  

# Thanks to All My Team Members, Cannot Win the Reward Without You!
![Reward](/images/TheReward.jpg)  
