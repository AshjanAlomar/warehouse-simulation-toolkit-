# warehouse-simulation-toolkit-
Steps of How to do a warehouse simulation toolkit  to create and save a map:

Because am using mac I had a trouble when am trying to download Ros and Ros packages so I use her the Ros Development studio ( http://rosds.online/ ) 

This is the source that I use to  do a warehouse simulation toolkit  to create and save a map in github :
1)	https://github.com/wh200720041/warehouse_simulation_toolkit.git 

the first thing that I did is to upload this files I upload  the file In $ simulation_ws/src/  and I compile the file  $ simulation_ws/ by 
``` $ catkin_make ```

1-	Simulation Description:

This package provides a simulation environment of warehouse. A robot is simulated at the center of the environment, with 2D laser scanner provided.

2-	Prerequisites:

Because I have mac as I mentioned befor so I didn’t download ros and ubuntu I just use it in the browser if you want to try it you can download Ubuntu 64-bit 18.04.
ROS Melodic. ROS Installation and the ROS Package that you need is 
``` $ sudo apt-get install ros-melodic-hector-trajectory-server ros-melodic-slam-gmapping ros-melodic-navigation```

3-	Launch ROS:

```$ roslaunch warehouse_simulation warehouse_simulation.launch```
now it’s launching the simulation so it’s waiting for the services and in order for us to see it we goanna open gazebo and this is it this is the simulation

![image](https://user-images.githubusercontent.com/86170422/123527611-a9d58980-d6e9-11eb-9f78-e42db49d1333.png)

so after launch that and to look at this we’re going to open up our Rviz (in graphical tools )

![image](https://user-images.githubusercontent.com/86170422/123527638-cbcf0c00-d6e9-11eb-8a4d-56b511e57f26.png)

4-	Robot Control:

You can use keyboard (arrow keys) to manually control the robot (select cmd window first) this is a part of the window after I control the robot a little bit 

![image](https://user-images.githubusercontent.com/86170422/123527647-e2756300-d6e9-11eb-8c7c-22b44bc77f84.png)


So you’re going to use this map in navigation so you’re going to want to save it so the last step is to save this map so we’re going to open up a new shell and we’re going to use the map server node in order to save it so here we’re going to type this command ``` $ rosrun map_server map_saver -f ~/map ```

![image](https://user-images.githubusercontent.com/86170422/123527701-4304a000-d6ea-11eb-8f4a-14bd28c31b9d.png)

And now you have your map ready to go . 



