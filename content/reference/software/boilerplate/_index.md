---
title: "Code Boilerplate"
---


## Subsystem

```java
package frc.robot;


import edu.wpi.first.wpilibj2.command.Command;
import edu.wpi.first.wpilibj2.command.InstantCommand;
import edu.wpi.first.wpilibj2.command.SubsystemBase;


public class Example extends SubsystemBase {


    private static Example m_instance;
    private ExampleStates m_state, m_lastState;


    public enum ExampleStates {
        IDLE("Idle");


        String stateName;


        private ExampleStates(String name) {
            this.stateName = name;
        }


        public String toString() {
            return this.stateName;
        }
    }


    public Example() {
        m_state = ExampleStates.IDLE;
    }


    public void periodic() {
        stateMachine();
    }


    private void stateMachine() {
        Command currentExampleCommand = null;
        if (!m_state.equals(m_lastState)) {
            switch (m_state) {
                case IDLE:
                    currentExampleCommand = Idle();
                    break;
                default:
                    m_state = ExampleStates.IDLE;
            }
        }


        m_lastState = m_state;


        if (currentDrivetrainCommand != null) {
            currentExampleCommand.schedule();
        }
    }


    private Command Idle() {
        return new InstantCommand();
    }


    public void setState(ExampleStates state) {
        m_state = state;
    }


    public final static Example getInstance() {
        if (m_instance == null) {
            m_instance = new Example();
        }
        return m_instance;
    }
}

```

[Source Document](https://docs.google.com/document/d/1kuAOz9eg85d1os2dZQnwEr1QmqcDwxQs6XTi003f00g/edit?usp=sharing)