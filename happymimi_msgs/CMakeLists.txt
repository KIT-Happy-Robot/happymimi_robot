cmake_minimum_required(VERSION 3.0.2)
project(happymimi_msgs)

find_package(catkin REQUIRED COMPONENTS
  message_generation
  sensor_msgs
  std_msgs
  std_srvs
)

## Generate messages in the 'msg' folder
add_message_files(
  FILES
  StrInt.msg
  SimpleBool.msg
)

## Generate services in the 'srv' folder
add_service_files(
  FILES
  StrTrg.srv
  SimpleTrg.srv
  SimpleString.srv
  SetStr.srv
  SetFloat.srv
  StrToStr.srv
  TwoFloat32Bool.srv
  Str2Str.srv
)

## Generate added messages and services with any dependencies listed here
generate_messages(
  DEPENDENCIES
  sensor_msgs
  std_msgs
)
catkin_package(CATKIN_DEPENDS sensor_msgs std_msgs std_srvs message_runtime)
