# Desktop Cleaning Robot

This project is based on the official competition demo. It is designed to autonomously clean desktops using computer vision and SLAM-based navigation, built on ROS.

## Features
- **Vision**: Detects and classifies objects based on color and shape using OpenCV, with a USB camera (`usb_cam`) for capturing visual data.
- **Sensors**: Equipped with ultrasonic and laser sensors for enhanced obstacle detection.
- **Mapping**: Builds real-time maps using Cartographer.
- **Navigation**: Utilizes Move Base and TEB local planner.

## Installation
1. Clone this repository.
2. Install dependencies.
3. Build the package:
   ```bash
   catkin_make
   source devel/setup.bash
   ```

## Usage
1. Mapping:
   ```bash
   ./scripts/cartographer_mapping.sh
   ```
2. Save the map:
   ```bash
   ./scripts/cartographer_save_map.sh
   ```
3. Run the cleaning operation:
   ```bash
   ./scripts/clean_desktop.sh
   ```
