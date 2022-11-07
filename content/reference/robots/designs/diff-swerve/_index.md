---
title: Differential Swerve
---

## What is Differential Swerve?

In a traditional coaxial swerve module module yaw (changing the heading of the wheel) and module transation (wheel rotation) are controlled by independent motors.

Differentail swerve uses the opposing rotation of the two drive motors to create translation and the rotation in the same direction to create yaw.

This video has a nice demo:
{{<youtube Y1XtXkTUXsI >}}

## Software
The software can easily become complex and diffucult to understand.

We found that using the simplyfing assumption that we should do our math in units of RPM causes a relativley simple set of formulas to fall out.

We found that two functions were needed:
1. Given the RPM of motor A and B determine the wheel translation RPM
2. Given the RPM of motor A and B determine the module yaw RPM

```java
    // Translation is calculated as half the difference of a and b,
    // adjusted by gear ratio. Translation is typically dependent on
    // all three pairs of gears. The differential pinion generates
    // translation as a function of the speed of the top and bottom
    // differential gears.
    double translationRPM = ((aMotorRPM - bMotorRPM) / 2) * GEAR_RATIO_WHEEL_SPEED ;
```
```java
    // Yaw is calculated as the average of a and b, adjusted by gear ratio
    double yawRPM = ((aMotorRPM + bMotorRPM) / 2) * GEAR_RATIO_YAW;
```

Full code example available on the team [GitHub under the DiffSwerve repository][1].

[1]: https://github.com/FRCteam4909/DiffSwerve/blob/2cb58aba940876eb6976fb47a586b4850e3382a5/src/main/java/frc/bionic/swerve/SwerveModule.java#L216-L242