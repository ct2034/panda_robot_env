# notes rosi workshop 09.10.19

## setup

1 roslaunch panda_env_bringup panda_env_bringup.launch
2 roslaunch moveit_setup_assistant setup_assistant.launch

gedit my_panda_moveit_config/config/panda.srdf
change second finger in group_state open ..

roslaunch my_panda_moveit_config move_group.launch

## jogging

rviz plugin +
`roslaunch panda_env_bringup jog_arm.launch`
