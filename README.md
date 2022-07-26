# set_up_ROS
in this repository I will explain the steps of ROS set up using virtual box and ubuntu

### first you need to download virtual box, ubuntu20.04, and ROS  

- to download virtual box click on the next link 
https://www.virtualbox.org/wiki/Downloads and set it up 

- to download ubuntu20.04 click on the next link 
https://releases.ubuntu.com/20.04/ 


# set_new_device  

1- launch vitual box and click on new button to create a new device 
![Capture 3](https://user-images.githubusercontent.com/108210044/181116744-f074fdbc-2a3b-4fdd-a221-120f69f9e351.PNG)



2- and type any name for your machine, I typed ros as the name, then click on next  
![Screenshot (661)](https://user-images.githubusercontent.com/108210044/181116878-b4858316-5d09-4f96-9024-0f4e15c7580f.png)
![Screenshot (660)](https://user-images.githubusercontent.com/108210044/181117467-775fe4e4-7260-4734-a88a-b670b32df7b3.png)
![Screenshot (662)](https://user-images.githubusercontent.com/108210044/181117478-93df44b9-04a9-40fd-8f4f-8fe0945eb7d6.png)
![Screenshot (663)](https://user-images.githubusercontent.com/108210044/181117481-b3f06967-d6b2-4190-a49b-ddfad17f52ca.png)
![Screenshot (664)](https://user-images.githubusercontent.com/108210044/181117485-0b3baaf6-ca93-4a7d-a4bf-8d1c3ad78cc8.png)



3- click on your machine and then start button 
do not change the default settings and click on next 
![launch_ROS_VB](https://user-images.githubusercontent.com/108210044/181118604-6712f67b-0d1e-426f-951f-822e862981ea.png)



# set_up_ubuntu 
1- from the folder select the ubuntu file you already download it, then click on start button 


2- intall ubuntu and keep clicking on next or continue 


3- set your name and password 

4- wait until all the set up thing end then click on restart 

5- when your virtual device is turned on search for the terminal from the search bar 

6- click on the terminal to type the next lines for ROS set up 



1.1- Setup your computer to accept software from packages.ros.org.

```
 sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
```

1.2- Set up your kyes 
```
sudo apt install curl # if you haven't already installed curl
curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
```

1.3- Installation 
```
sudo apt update
```
```
sudo apt install ros-noetic-desktop-full
```
```
sudo apt install ros-noetic-PACKAGE
```

1.4- enviroment set up 
```
source /opt/ros/noetic/setup.bash

echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
source ~/.bashrc


```


1.5- Dependencies for building packages

```
sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential
```

1.6- Initialize rosdep

```

sudo apt install python3-rosdep

sudo rosdep init
rosdep update

```





