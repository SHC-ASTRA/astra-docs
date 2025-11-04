# ROS2 Repository Name

Brief description of what the repository is for.

This is a template

## Table of Contents

- [Software Prerequisites](#software-prerequisites)
- [Usage](#usage)
  - [Setup](#setup)
    - [Nix](#nix)
    - [ROS2 Humble + rosdep](#ros2-humble-rosdep)
  - [Running](#running)
- [Packages](#packages)

## Software Prerequisites

List of things you need set up and working with links to the things. Do not list
dependencies, instead list things that need to be set up (e.g. Nix, ROS2 Humble,
Visual Studio Code, PlatformIO, etc). Include links to setup instructions. Here's an example:

You need either [ROS2 Humble](https://docs.ros.org/en/humble/Installation.html)
with [rosdep](https://docs.ros.org/en/humble/Tutorials/Intermediate/Rosdep.html#rosdep-installation)
or [Nix](https://nixos.org/download/#nix-install-linux) installed. We recommend
using Nix.

## Usage

Here are some example usage instructions for a ROS2 repo.

### Setup

#### Nix

With Nix, all you have to do is enter the development shell:

```bash
cd path/to/repo/
nix develop
```

#### ROS2 Humble + rosdep

With ROS2 Humble, start by using rosdep to install dependencies:

```bash
cd path/to/repo/
rosdep install --from-paths src -y --ignore-src
```

### Running

First, build the package:

```bash
colcon build
```

Second, run the package:

```bash
source install/setup.bash
ros2 launch example_pkg example.launch.py
```

## Packages

Include a list of the packages inside the repository here.

- [example\_pkg](./example_pkg) - Does example things.
