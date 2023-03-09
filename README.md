# Finding Things in the Unknown: Semantic Object-Centric Exploration with an MAV

This repository contains the code and simulator for the ICRA 2023
paper “Finding Things in the Unknown: Semantic Object-Centric
Exploration with an MAV”.

For more information see the [paper](https://arxiv.org/abs/2302.14569) and
[video](https://youtu.be/z0LVe_8SATU).

``` bibtex
@InProceedings{Papatheodorou_ICRA2023,
  author    = "Papatheodorou, Sotiris and Funk, Nils and Tzoumanikas, Dimos and Choi, Christopher and Xu, Binbin and Leutenegger, Stefan",
  title     = "Finding Things in the Unknown: Semantic Object-Centric Exploration with an {MAV}",
  booktitle = "IEEE International Conference on Robotics and Automation",
  address   = "London, United Kingdom",
  year      = "2023",
  month     = "May",
}
```

Work-in-progress. Check again in a few days for the source code.


## Setup

The code has been tested on Ubuntu 20.04 and ROS Noetic. Install
the `ros-noetic-desktop-full` package by following the
[ROS Noetic installation instructions](http://wiki.ros.org/noetic/Installation/Ubuntu)
and then install the dependencies:

``` sh
sudo apt-get --yes install git g++ cmake libeigen3-dev libopencv-dev libyaml-cpp-dev python3-catkin-tools
```


## Build

``` sh
# Create and initialize a new catkin workspace.
source /opt/ros/noetic/setup.bash
mkdir -p ~/exploration_ws/src
cd ~/exploration_ws
catkin init

# Clone this repository and all submodules.
cd ~/exploration_ws/src
git clone --recurse-submodules https://github.com/smartroboticslab/semantic-exploration-icra-2023.git

# Build all ROS packages.
catkin build -DCMAKE_BUILD_TYPE=Release
source ~/exploration_ws/devel/setup.bash
```


## Usage

TODO (dataset download, launch files)


## License

See the individual submodules for their license terms.
