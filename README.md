# Mouse Node Package

## Overview

The Mouse Node Package is a ROS package that reads data from `/dev/input/mouse0` and publishes it to a ROS topic. This package is designed to demonstrate a simple ROS node that interfaces with mouse input.

## Prerequisites

- ROS (Robot Operating System): Melodic or Noetic
- Linux system with `/dev/input/mouse0` available (typically available on most Linux systems)

## Installation

1. Clone this repository into your Catkin workspace's `src` directory:

    ```bash
    git clone https://github.com/sedenmutaf1/mouse_node_seden.git
    ```

2. Build your Catkin workspace:

    ```bash
    cd ~/catkin_ws
    catkin_make
    ```

3. Source your workspace:

    ```bash
    source devel/setup.bash
    ```

## Usage

1. Run the Mouse Node:

    ```bash
    rosrun mouse_node_seden mouse_node
    ```

2. Monitor the Published Data:

    Subscribe to the `/mouse_node` topic to view the published mouse data. You can use tools like `rostopic echo` or `rqt_console`.

## Example

To visualize the data published by the mouse node, you can use the following commands:

```bash
rostopic echo /mouse_node
