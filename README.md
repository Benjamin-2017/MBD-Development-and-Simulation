# MBD-Development-and-Simulation
1   Design and Simulation Environment
using Pilot Input Device,MATLAB/SIMULINK,FlightGear to develop a airplane Design and Simulation Environment. 

(1) the Pilot Input Device include Yoke for Elevator and Aileron Control, Rudder,and Throttle

![](https://github.com/Benjamin-2017/MBD-Development-and-Simulation/blob/master/Yoke.jpg)
![](https://github.com/Benjamin-2017/MBD-Development-and-Simulation/blob/master/Rudder.jpg)
![](https://github.com/Benjamin-2017/MBD-Development-and-Simulation/blob/master/Throttle.jpg)


(2) using MATLAB 2019a to develop FlightController and FlightDynamic Model.

![](https://github.com/Benjamin-2017/MBD-Development-and-Simulation/blob/master/SimulinkModel.jpg)



(3）using FlightGear to display aircraft motion and flight trajectory.
 I linked the Model to two FlightGears,one for Local Computer display,another for Remotely Computer display via UDP.
 
 ![](https://github.com/Benjamin-2017/MBD-Development-and-Simulation/blob/master/LocalFlightGear.jpg)
 ![](https://github.com/Benjamin-2017/MBD-Development-and-Simulation/blob/master/RemotelyFlightGear.jpg)
 
 
（4）overall Architecture
 The Required Hardware and software environmennt are built  as follows:

 ![](https://github.com/Benjamin-2017/MBD-Development-and-Simulation/blob/master/OveralSchematicdiagram.jpg)

 
 there are several technical concearns to be resolved before the simulation system can work.

 2  interfaces between Input Devices and MATLAB/SIMULINK,and FlightGear

 in the traditional simulation ,there are just one input device and one flightgear linked to Simulink Model.
 But I used two set input devices to implement more input signals function. and also two FlightGears are shown to display flight path    and flight deck inside the cockpit.
 
 2.1 interfaces between Input Devices and MATLAB/SIMULINK
 input devices:Flight Yoke System,Flight Rudder Pedals,and Throttle Quadrant.
  two interface Modules in Simulink are used to interpret the input data.
  ![](https://github.com/Benjamin-2017/MBD-Development-and-Simulation/blob/master/input_interface_function.JPG)
 
 
 2.2 interfaces between  MATLAB/SIMULINK and FlightGears
 The Simulation Results are transimitted to Local FlightGear and Remotely FlightGear to show more flight details.
 
 there are two inferface function in Simulink to link to Local FlightGear and Remotely FlightGear.
  ![](https://github.com/Benjamin-2017/MBD-Development-and-Simulation/blob/master/twoFightGears_interface_function.JPG) 
 
 
 2.3 Flight Dynamic Model
 
 when the aircraft flight dynamic Model is fully completed,you can fly it as follows:
  ![](https://github.com/Benjamin-2017/MBD-Development-and-Simulation/blob/master/fly.jpg) 
 
 
 
 
 
 
 
 
 
 
 
 
 








