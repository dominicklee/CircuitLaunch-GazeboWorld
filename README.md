# CircuitLaunch Gazebo World
Experiment with your ROS/ROS2 robots with a Gazebo world of Circuit Launch

## Overview
Using a 2D layout, provided courtesy of Alex Dantas (CEO of CircuitLaunch), I have created an approximate digital version of the building as a Gazebo world. This simulation enables roboticists and engineers to test their robots from anywhere prior to real-world experiments.

For GyroPalm's use-case, this enables users to experience the joy of controlling a digital robot and practice performing driving and gestures without the risk of potential robot collision. By using this repository, you agree to use the files at your own risk and understand that real-world conditions may vary. Dimensions are approximate and subject to change without notice.

## Installation
Copy the `circuit_launch` folder to your own `building_editor_models` in your user directory. If you do not have a `building_editor_models` directory, create a new one. Also copy the `CircuitLaunch2024.world` to your user directory.

Ensure you have Gazebo installed. Then open a terminal and run:
```bash
gazebo CircuitLaunch2024.world
```

If Gazebo freezes or asks you whether to "Force Quit" or "Wait", keep clicking "Wait" until the world fully loads. This may take up to 5 minutes since the building is large.

## Troubleshooting
If Gazebo continues to freeze after 5 minutes, hit `CTRL+C` in your terminal. Then run this to ensure Gazebo is fully closed:
```bash
killall -9 gzserver
```

Afterwards, try again to open Gazebo.
