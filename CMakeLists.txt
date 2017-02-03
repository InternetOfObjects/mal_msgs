cmake_minimum_required(VERSION 2.8.3)
project(mal_msgs)

find_package(catkin REQUIRED COMPONENTS
  std_msgs
  message_generation
  )

add_message_files(
  FILES
  ArmServoMovement.msg
  ArmServoState.msg
  ArmServoStates.msg
  LegServoMovement.msg
  LegServoState.msg
  LegServoStates.msg
  Movement.msg
  )

generate_messages(
  DEPENDENCIES
  std_msgs
  )

