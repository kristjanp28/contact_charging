cmake_minimum_required(VERSION 2.8.3)
project(contact_charging)

find_package(catkin REQUIRED)

catkin_package(
	CATKIN_DEPENDS std_msgs geometry_msgs sensor_msgs
)

install(PROGRAMS
	scripts/contact_charging.py
	DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)