# Clone
- Create a workspace named `ascam_ros2_ws/src`
- Clone this repo
- Build

# Build
`colcon build --symlink-install --cmake-args -DCROSS_COMPILE=x86_64-linux-gnu`

# Install udev rules
- `cd ~/ascam_ros2_ws/src/ascamera/scripts`
- `sudo bash create_udev_rules.sh`

# Update the config file path
- `cd ~/ascam_ros2_ws/src/ascamera/configurationfiles`
- edit configuration file path in `hp60c.launch.py`

# Launch
- `ros2 launch ascamera hp60c.launch.py`

# View images
- `ros2 run rqt_image_view rqt_image_view`
- `rviz2`

# Frame ID
- ascamera_hp60c_color_0 (for rviz)
