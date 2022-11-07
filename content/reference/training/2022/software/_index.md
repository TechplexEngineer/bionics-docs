---
title: 2022 Software Training
description: 2022 Software Preseason Training
# weight: 10
---

We divided our large group based on the results of a survey into two groups. An intro level grou with little to no programming expereince and, an Advanced level with some programming experience. The focus for the intro level grou was to come up to speed with Java programming and the FRC Control System. The Advanced group focused on the FRC control system and higher level concepts such as PID and Commands.

## Intro Level "Concepts Group"

### Week 1-2
Objective: Familiarize them with basic programming concepts
- Blockly and basic concepts (https://blockly.games/ Maze and Turtle)
	+ Statements
	+ Loops
	+ Conditionals
	+ Types
	+ Number, String, etc.
	+ Variables
	+ Functions
### Week 3-4
Objective: Intro to setup and periodic using Elevator Simulator
- [Directions](https://docs.google.com/document/d/14gCJyj_c6jQDQC8Owub1HoIApCRfR18DalbGPCFk2kM/edit)
- [Elevator Simulator](https://derrell.github.io/frc-elevator-sim/output/source/)
### Week 5-6
Objective: Introduce them to basic Java programming with ROMI
- Relate basic concepts from Blockly to how done in Java
	+ Specific Java types vs generic Blockly types
		* int and float and double, etc. vs Number
- Intro to Object Oriented
- Show them the [Slides](https://docs.google.com/presentation/d/1MxjAYEkdW9MVuQUSKM9xFdQ3vQl-1MXcdd2jdfOI_KY/edit#slide=id.p) and have them follow along on their own computers.
- Implement hands-on exercises from slides, using jdoodle
### Weeks 7-N
Objective: Get them set up and familiarized with all the necessary tools.
- Introduction to WPILIB Vscode
- Introduction to WPILIB Documentation and how to use it.
Objective: A basic understanding of FRC programming
- Work in groups (depends on no. of people) to use Romi to measure distance with encoders.
- Stretch goals
	+ Have Romi drive a set distance and stop when the desired distance is reached.


### Romi Tasks
Romi tasks are:
- Code walk-through; comparison with Elevator Simulator
- Control motor via A (forward direction) and B (backward direction) button
- Crash if teleop -> disable -> teleop (teleopInit vs robotInit)
- Add "Right" motor
- Move Romi forward, move backward via A and B buttons
- Autonomous: drive forward for 3 seconds
- Encoder experiments
- Autonomous: 24" move
- Correct motor speed difference with a multiplier
- Autonomous: 24" move then return
- Autonomous: rotate using gyro
	+ Needs RomiGyro class which is in their repo on the three Training computers (obtained from https://github.com/derrell/romi-training-01.git) under romi-training-01/advanced/main/java/frc/robot/sensor/RomiGyro.java. That file has been kept out of source tree to avoid confusion for early work, but will now need to be moved into `src/main/java/frc/robot/`.
- All Romi tasks except the last one are accomplished solely in Robot.java. Avoiding complication of classes.
There is example code showing how each of the above tasks are done, although not identified specifically by the above Romi tasks. The example code is at https://github.com/derrell/romi-examples.git. There is a separate branch for each example, called - exercise-1, exercise-2, ... exercise-7.


## Advanced Level "FRC Group"

### Week 1
Objective: Get them set up and familiarized with all the necessary tools.
- Introduction to Github, creation of GitHub accounts.
- Introduction to WPILIB VsCode, installing it onto any laptops that don’t have 2021.
- Introduction to WPILIB Documentation and how to use it.

### Week 2-5
Objective: Work with Romi building on template code, writing their first robot program.
- Assemble two Romi’s (Be careful with the tab when pushing the motor into the base)
- Work in groups (depends on no. of people) to use Romi to measure distance with encoders.
- Have Romi drive a set distance and stop when the desired distance is reached.
- Stretch goals:
	+ Use IMU (Accelerometer and Gyro) to determine angle and acceleration of Romi and display it.

### Week 5 (May go into 6)
Objective: Write their first robot program from scratch.
- Write code for a Spark to make a motor spin on a button press.

### Week 6-8
Objective: Expand on their code
- Write code so the motor spins in reaction to a REV Color Sensor detecting something.
- Stretch goals:
	+ PID understanding (and implementation?)
	+ Different speeds depending on different joystick inputs
	+ Try with a pixycam (speed up depending on how many balls are detected)
