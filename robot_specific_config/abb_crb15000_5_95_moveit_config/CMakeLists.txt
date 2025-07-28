cmake_minimum_required(VERSION 3.10.2)
project(abb_crb15000_5_95_moveit_config)

# This package provides MoveIt configuration files for the ABB CRB 15000
# collaborative robot (5 kg payload with 0.95 m reach).  It follows the same
# structure as the IRB‑1200 MoveIt package included in this repository and
# installs configuration and RViz files into the share directory.

find_package(ament_cmake REQUIRED)

ament_package()

install(
  DIRECTORY config rviz
  DESTINATION share/${PROJECT_NAME}
)