---
title: Drivetrains & Wheels
description: Common wheel and chassis configurations
---

The best drive train:
- is more **important** than anything else on the robot
- meets your **strategy** goals
- can be build with your team **resources**
- rarely needs **maintenance**
- can be **fixed** within 4 minutes
- is more **important** than anything else on the robot

Basics
- Know your resources (manufacturing, cost, design, etc)
- Use strategy to inform choices:
    + Speed, power, shifting, mobility
- Use most powerful motors on drive train
- When testing the drive train, **weigh it down**. (Don't drive 1/2 the robot)
- Stress test early, implement fixes (not duck-tape and super-glue)
- Give software **TIME to work**
- Give drives **TIME to drive**
- Plan for sensor locations early

Src: [^2008-baker-drive-systems]

## Types of Wheels
There are a lot of wheels that get used in FRC, here are some classic choices and their use cases.

### The Colson Wheel
{{< figure src="colson-wheel.jpg" alt="Colson Wheel" height="250px" >}}

The colson is a classic wheel, with some good characteristics. It’s commonly available with a .5" hex bore from VEXPro, and other suppliers without a .5" hex bore (but VEX sells a press-fit insert for the bore).

Pros:

- Low maintenance - service for this wheel is most commonly “remove and replace”
- Good traction - provides relatively good traction on the field carpet, and stands up to defense.
- Good mobility - allows for a robot to turn relatively easily.
- Sizes - available in many sizes (both width and diameter), allowing for different mechanism characteristics and gearing.

Cons:

- Wears quickly - colsons used in traction applications
- Expensive - especially for a part which wears quickly, colsons are relatively expensive.
Heavy - colsons are relatively heavy wheels
- Not extremely compliant - the tread is typically not very “compliant”, and given the aluminum hub it doesn’t really deflect very much when encountering a game piece.

**The bottom line:** colsons provide an excellent choice on drive trains, and commonly used as a 4x1.5 size for west coast style drivetrains. They provide good traction with few tradeoffs. Some teams also use colsons for their flywheels for powered shooters, with success. Colsons have been used by teams for years, at the highest level of play in FRC.

### The "traction wheel" (aluminum hubs + tread)
{{< figure src="traction-wheel.jpg" alt="traction wheel" height="250px" >}}

The traction wheel is also a classic drive train or light mechanism choice, with excellent drive characteristics. It is available in many sizes, and from multiple suppliers (commonly VEXPro, WCP and AndyMark).

Pros:
- Great traction - provides excellent traction on field surface, and stands up well to defense.
- Good mobility - allows for robot to turn relatively easily.
- Sizes - available in many sizes.
- Weight - most hubs have a large amount of open space, and therefore are relatively lightweight.
- Re-usability - hubs can be reused from year to year, provided new traction material is applied.

Cons:

- High maintenance - the tread can wear quickly, and replacing tread can be a hassle. Tread if not secured can also come off during a competition, rendering the robot effectively traction less.
- Expensive - hubs alone typically cost in the 15-20 dollar range, per wheel. Although they can be easily reused, tread also starts to add to the cost. Initial investment for an 8wd would be close to the $300 range, which is rather expensive for especially newer teams.
- Not extremely compliant - the tread is typically not very “compliant”, and given the aluminum hub it doesn’t really deflect very much when encountering a game piece.

**The bottom line:** traction wheels are great in drivetrains, but their cost, traction surface and lack of compliance makes them a hard choice for most manipulators. They are a first-rate choice for many teams for drive trains, and have been season tested for years by many teams at the highest level of play.

### The Mecanum wheel
{{< figure src="mecanum-wheel.jpg" alt="Mecanum wheel" height="250px" >}}

The mecanum wheel allows for drivetrains to strafe (that is, move directly left-right and right-left), but provide very low traction on field surface and make teams incredibly susceptible to defense. Their vectoring characteristics make them a great choice for intakes for some game pieces. They are commonly available from AndyMark and VEXPro, with a 3d-printed version available here on chief as well.

Pros:
- Vectoring surface - these wheels allow intakes that move a game piece across the robot, allowing for teams to design a single cutout in their bumpers / robot, and have game pieces travel to that location.
- Strafing - if used in a drivetrain, this wheel allows robots to strafe directly to the left and right, without turning the robot.

Cons:
- Low traction - these wheels effectively provide zero traction on the field surface, and leave robots out to heavy defense.
- Heavy - many mecanums are very heavy, as they depend on several shafts inside the mecanum.
- Cost - unless you are 3d printing your mecanums (which is hard to do for a drivetrain), they are very expensive, around $30 / wheel.

**The bottom line:** not a popular choice for drivetrains, just based upon their lack of traction. They are great for intakes for some game pieces (2016/2020 had great game pieces for this), but intakes with them can be expensive and hard to set up.

### The omni wheel
{{< figure src="omni-wheel.jpg" alt="omni wheel" height="250px" >}}

The omni wheel is similar to a mecanum, allowing for robots to move directly sideways. However, since it is lower profile and has a slightly different geometry, it is sometimes placed in drivetrains with other traction wheels (usually 2 in the front or rear corners, commonly referred to as “4x2”, “6x2” or sometimes “2x2”). They are commonly available from VEXPro and AndyMark.

Pros:
- Incredible turning characteristics - if placed in corners, this can save some bad design, or allow teams to make otherwise very flat drivetrains.
- Good game piece manipulation - allows for game pieces to be coming in at an angle, but still move them forward. Great in a mecanum intake, as the middle wheel.
- Re-usability - can be reused from season to season with relatively low wear.

Cons:

- No traction - again, with roller surface, these wheels have effectively no traction
- Relatively weighty - about as heavy as a colson for some wheels, omnis can be weighty.
- Expensive - again, about $20-$30 for each wheel.

**The bottom line:** omnis are frequently used in drivetrains, with other traction wheels on the robot. This allows for these robots to turn a little better, or other positive drivetrain characteristics.

### The compliant wheel
{{< figure src="compliant-wheels.jpg" alt="compliant wheel" height="250px" >}}

Compliant wheels are very squishy, and allow for great control of game pieces - particularly those that are rigid in nature (2015/2018/2019). They are not a good choice for drive trains, as they deform too much. They are typically available from AndyMark and Banebots.

Pros:
- Very flexible - at certain durometers, these wheels flex a lot. This really helps pickup rigid items.
- Price - they are relatively cheap
- Weight - they are very light, and have little material

Cons:
- Not a drive wheel - in FRC, robots are simply too heavy to use these as a drive wheel.
- Deformation - at high speeds, these wheels tend to expand a lot, which can create some deformation problems or different intake characteristics than expected.

**The bottom line:** compliant wheels are great in manipulators, especially for a firm or rigid game piece.

### The Hi-Grip wheels
{{< figure src="hi-grip-wheels.jpg" alt="Hi-Grip wheels" height="250px" >}}

The hi-grip wheels are commonly available from AndyMark, and are familiar to most teams as "the kitbot wheels". They are relatively high performance, and have been battle tested drivetrain wheels at even the highest level of play.

Pros:
- Good traction - these wheels provide good traction on the field surface.
- Inexpensive - these wheels are relatively cheap.
- Many sizes - these wheels are offered in several sizes, from 4-8 inches.
- Weight - for their size, these wheels are relatively lightweight.

Cons:
- Plastic hubs are weak - these wheels can sometimes crack under pressure, so have spares ready.
- Wear and tear - these wheels tend to wear down quickly, and should be replaced every couple of events.
- Relatively thin - they are only available in one thickness, and are relatively thin. This makes them more susceptible to defense.

**The bottom line:** if you’ve been a rookie, or used the KOP drivetrain, you’ve used these wheels. They are high performance, inexpensive, and get the job done without frills. They are an excellent choice for most drivetrains, and are more than serviceable even at high levels of play.

### The pneumatic wheel
{{< figure src="pneumatic-wheels.jpg" alt="pneumatic wheel" height="250px" >}}

This is an air-filled wheel with good traction, and can take a beating. The extra air cushion that these wheels offer makes them great for rough terrain (2016), and they have excellent traction. They are commonly available from VEXPro and AndyMark.

Pros:
- Lots of traction - these wheels are sticky, and hard to play defense against.
- Can take a beating - they can send over rough terrain without issue, and bounce along for a drivetrain.
- Serviceability - service for these wheels is typically “ensure they’re inflated right”, and you’re off to the races.

Cons:
- Expensive - this 8" variety is $65/wheel from AndyMark.
- Too much traction - poorly designed drivetrains, or drivetrains without some considerations suffer from a lack of turning when using these wheels.

**The bottom line:** while good for rough terrain, these wheels are quite the price tradeoff in a year which does not depend on your ability to cross terrain like that faced in 2016. They don’t make a great choice in intakes due to their size, and for shooters they aren’t well recommended due to the fact that they are an air filled tire.

Source [^2021-cd-macaig]

## Types of Drivetrains
Drivetrains combine wheels and chassis elements to provide a movable foundation for robots.

### Tank Drive
Tank Drives are very common in the FRC community. 

- Left and right sides are driven independently
- Often the center wheels are dropped 1/16" - 3/16" to make turning easier

Pros:
- Simple & inexpensive
- Software well supported
- Easy to drive
- Potential for high pushing force

Cons:
- Less agile than other drivetrains
    + Can be diffucult to turn.

#### West Coast / Live Axle
A West Coast drivetrain is a type of tank drive where the wheel axles are only supported on one side.
- cantilevered wheels
- allows for wider robots

### Omni-directional drivetrains

#### Swerve / Crab
- Wheel modules rotate on vertical axis to control direction
- typically four traction wheels, one in each robot corner

Pros:
- Potential for high speed and/or pushing force
- Very Agile (can move in all directions)
- Simple wheels

Cons:
- Requires custom modules and extra motors (2 per module)
- Very complex, expensive to build
- Challenging to program
- Heavy when compared to tank drive

#### Slide / H-Drive
- Similar layout to tank dive
- Uses only omni-wheels

Pros:
- Fairly easy to design & build (Note: Critical for wheels must be on the same plane. Easier with CNC machining)
- Very Agile (can move in all directions)

Cons:
- Very little potential pushing force
- Extra wheel(s)/motor(s)/gearbox(es) required

#### Mecanum
- Similar layout to tank drive
- Each wheel must be driven independently
- Must use 4 mecanum wheels

Pros:
- Fairly easy to design & build (Note: Critical for wheels must be on the same plane. Easier with CNC machining)
- Very Agile (can move in all directions)

Cons:
- Wheels are expensive
- Extra motor(s)/gearbox(es) required
- Minimal braking ability
- Difficulty on inclines
- Very little potential pushing force
- Challenging to program & drive

#### Holonomic Drive
- 4 omni wheels at 45° or 3 at 120°
- Each wheel must be driven independently

Pros:
- Agile
- Immediate turning
- Easy to design and build

Cons:
- No brakes
- Difficulty on inclines
- Very little potential pushing force
- Challenging to program and drive
- Extra motor(s)/gearbox(es) required

## Robot Speed
- Too Fast
    + won't have enough torque to move
    + Leading to hard to control
- Too Slow
    + too much torque causing wheels to slip
    + too slow to be effective

Rule of thumb:
- Single speed gearbox, 8-12 ft/s
- Two speed gearbox, 18 ft/s to 4 ft/s

### Wheel Size
Wheel Size can have a large impact on your design.

- Smaller Wheels
    + Less gear reduction needed
    + less weight
    + Lower center of gravity (less prone to tipping)
- Larger Wheels
    + Lower RPM for the same linear velocity (less tread wear)
    + Larger sprocket to wheel diameter ratio (less tension on chain/belts)

### Number of wheels

{{<columns markdown="true">}}
##### 2 Wheel Drive
Pros:
- low resistance turns

Cons:
- challenging to drive
- easily defended
- lower pushing force (less friction)
- may not turn at robot center
<--->
##### 4 Wheel Drive
Pros:
- long wheel base

Cons:
- One set of wheels needs to be omni
- challenging to drive
- easily defended
- lower pushing force (less friction)
- may not turn at robot center
<--->
##### 6 Wheel Drive
Pros:
- great turning with high traction wheels with dropped center
- full pushing force potential

Cons:
- extra wheels add weight
<--->
##### 8 Wheel Drive
Pros:
- great turning with high traction wheels with dropped center
- full pushing force potential

Cons:
- extra wheels add weight
- more power transmission complexity.
{{</columns>}}
Source [^2013-zhu-drivetrains]


## Drivetrain Simulator
Many teams have built drivetrain models, one particularly good one is [ILITE Drivetrain Simulator][4]



[^2021-cd-macaig]: [Chief Delphi: What are different types of wheels good for?][1]
[^2013-zhu-drivetrains]: [Presentation: Introduction to Drivetrains][2]
[^2008-baker-drive-systems]: [FIRST Robotics Drive Systems by Andy Baker (2008)][3]

[1]: https://www.chiefdelphi.com/t/what-are-different-types-of-wheels-good-for/393828/7
[2]: https://prezi.com/4bw1pdf7-pgj/introduction-to-drivetrains/
[3]: https://www.andymark.com/pages/presentations
[4]: https://www.chiefdelphi.com/t/ilite-drivetrain-simulator-v2020/369188

