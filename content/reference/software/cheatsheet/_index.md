---
title: "Java Cheat Sheet"
date: 2023-01-18T10:47:28-05:00
draft: false
---


## Sample Java Class
```java
// A package is a group of Java Classes
package frc.robot;

// Imports tell the compiler to bring in references to other classes
import frc.robot.subsystems.DrivetrainSubsystem;

// create a class which is a grouping of data and methods called "Module"
public class Module {

	// class variable, can be used inside the class
    String m_name;


    // Constructor method. Has no return type, and has the same name "Module" as the class "Module".
    public Module(String name) {
        this.m_name = name;
    }
  
  	// Method. Takes no parameters, and returns a double.
    public double getHeading() {       
    	return 90.0;
    }

    // Method. Takes two paramaters "a" of type double, and "b" of type double
    public double add(double a, double b) {
    	// add a and be and give that to the caller.
    	return a + b;
    }

}
```

