This directory contains the specific CAD models of the AGV, which are used in the URDF description of the mobile robot.
Links are in the folders with their respective names, the entire assembly is saved in the assembly folder.



ros2 run xacro xacro \
  $(ros2 pkg prefix agv_pus_description)/share/agv_pus_description/urdf/mech/agv_base.urdf.xacro \
  > /tmp/agv_base.urdf

ros2 launch urdf_tutorial display.launch.py model:=/tmp/agv_base.urdf

za vizualizacijo posameznih linkov (mors mu dat tudi ime)

Linux /tmp is usually cleared on reboot automatically.

ros2 launch urdf_tutorial display.launch.py model:=/home/ziga/ros2_ws/src/agv_pus/agv_pus_description/urdf/robots/agv_pus.urdf.xacro 