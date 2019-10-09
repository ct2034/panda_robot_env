# notes rosi workshop 09.10.19

## setup

1. `roslaunch panda_env_bringup panda_env_bringup.launch`
2. `roslaunch moveit_setup_assistant setup_assistant.launch`
  * Create new
  * browse for urdf
  * self collisions - genrate
  * planning groups
    * add group arm
    * ik: kdl
    * add chain: panda_link_0 until link_9 
    * add group hand
    * no ik
    * add joint hand, finger1, finger2
  * poses: any, eg open and closed for hand
  * end effector add with name like hand
  * passive joint: finger 2
  * author

`gedit my_panda_moveit_config/config/panda.srdf`
change second finger in group_state open ..

roslaunch my_panda_moveit_config move_group.launch

## jogging

rviz plugin +
`roslaunch panda_env_bringup jog_arm.launch`
