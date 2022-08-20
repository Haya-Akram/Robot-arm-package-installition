**What is** **a Robotic Arm?**

![images](https://user-images.githubusercontent.com/109688460/185763924-56a3a736-5be8-42c2-9eaf-1d73b8bfc62d.jpg) ![download](https://user-images.githubusercontent.com/109688460/185763824-98bd66c8-ead3-4483-8312-251fb22338b0.jpg)

> A robotic arm is a type of mechanical arm, it has similar functions to a human arm, so it is extremely useful in industry as well as personal settings for assembly, drilling, machining, pick-and-place, and other applications.

**The steps to install robot arm package :**
1. **Firstly**, create a workspace to install the arm package on it.
   >  so start with create a new folder with the name **catkin_ws** \ (ws is a shortcut os WorkSpace)
        **by** this command:  `mkdir -p ~/catkin_ws/src`
2. **Change** the directory to the folder we created now by : `cd ~/catkin_ws/`
    then: `catkin_make`
              `cd ~/catkin_ws/src`
3. **Download** the packages insdie catkin_ws folder from this link: `git clone https://github.com/smart-methods/arduino_robot_arm.git `
4. **Go** to the workspace we was created to install ROS dependencies by use this command : `cd ~/catkin_ws `
then do all these commands by order: 
`rosdep install --from-paths src --ignore-src -r -y`
`sudo apt-get install ros-noetic-moveit`
`sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui`
`sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher`
`sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control`

5. **Now** add this line `sudo nano ~/.bashrc` to edit the file **bashrc**
6. **Then** use this line: `source /home/"username"/catkin_ws/devel/setup.bash` , which has location of workspace we was created in
7. **to save**the changes and finish, so press `ctrl + o` ---> `ctrl + X`
8. **Update** the source file of bashrc by  this command: `source ~/.bashrc`
9. **In the end**, launch **RIVz** by this command: `roslaunch robot_arm_pkg check_motors.launch`
> 
![rivs](https://user-images.githubusercontent.com/109688460/185763612-9aadf4e9-84a1-4a5a-9996-e11ad3a7bd7d.PNG)


****
