## Low-Cost touch screen Medical Monitering System 

#### Project Specifications:
This project is the final phase in the development of a low cost,
portable, medical monitoring system. In the previous phases of
the project, we built a simple kernel and utilized a nonpreemptive schedule to manage the selection and execution of
the set of tasks comprising our system. We took the first steps
towards implementing and incorporating the Peripheral
Subsystem by replacing several of the modeled / simulated measurement capabilities with the
initial design of the drivers to support the specified tasks and developed the initial support for
the Intrasystem Communication Channel.
We have also taken the initial steps toward developing the user interface by extending the
TFT keypad display. Finally, we improved the overall flow of control, and enhancing the
safety of the system.
The goal of this phase of the project is to continue and to extend our development of the
medical monitoring system. To that end, we’ll work with some of the other built in
capabilities on the UNO and ATMega 2560 microcontrollers.
The final subsystem must be capable collecting data from several different types of sensors,
processing the data from those sensors, displaying it locally, and then transmitting it over a
local area network to a collection management station. In the final phase of the design life
cycle for the project, we will now,
1. Add features and capabilities to an existing product.
2. Amend the formal specifications to reflect the new features.
3. Amend existing UML diagrams to reflect the new features.
4. Incorporate several additional simple tasks to our system.
5. Work with a hard real-time constraint on one of the tasks.
6. Learn and work with some digital signal processing tools.
7. Introduce additional peripheral devices and develop drivers for them.
8. Introduce and manage a formal communication protocol.
9. Incorporate additional safety components into the system. 

System Requirements Specification
1.0 General Description
A low cost, state of the art medical monitoring and analysis system is to be designed and
developed. The following specification elaborates the requirements for the display and alarm
portion of the system.
The display and alarm management subsystem must accept inputs from a number of sensors
used to collect data from various parts of the human body and signal a warning if the data
falls outside of pre-specified bounds. Some analysis of the data will be performed by other
parts of the system to be designed later.
The outputs of the sensors that are measuring a variety of natural phenomenon comprise a
number of different data types such as integers, strings or high precision numbers. The
system must be designed to accommodate each of these different types.
2.0 Medical Monitoring System
Description Modified
Displayed messages comprise three major categories: annunciation, status, and warning /
alarm. Such information is to be presented on the System Control TFT display and on a
series of lights on the Peripheral Subsystem front panel.
Sensor signals are to be continuously monitored against predetermined limits. If such limits
are exceeded, a visible indication is to be given and shall continue until acknowledged.
Acknowledgement shall terminate the initial indication but an alternate visible indication
shall continue until the aberrant value has returned to its proper range. If the signal value
remains out of range for a specified time, the primary annunciation shall recommence.
The local display function will be fully incorporated during this phase. 
- 5 of 26 -
System Inputs
The display and measurement component of the system in the first prototype must track
and support the measurement and display of the following signals:
Measurements
Blood Pressure
Body temperature
Pulse rate
Phase II Addition
Keypad Data
Measurement Selection
System Outputs
The display component of the system must track and support the display of the following
signals:
Measurements
Blood Pressure
Body temperature
Pulse rate
The status, alarm, and warning management portion of the system must monitor and
annunciate the following signals:
Status
Battery state
Warning
Temperature, blood pressure, or pulse rate out of range
Alarms
Temperature, blood pressure, or pulse rate in dangerous range 
