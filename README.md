# multirotor-related-tasks
This repository features a collection of multi-rotor related tasks: path planning on Ardupilot Mission Planner, YOLOv7 training for alphanumeric detection and a python script that outlines further processing,  and a rough scheme for how the hardware should be connected .

RoboFlow was used for custom trained dataset with classes for alphanumerics which was then fed them into YOLOv7 model and accuracies were reported . 
For the connections,
Flight controller: The Cube Orange+ (PixHawk): Connect the Cube Orange+ flight controller to your mainboard or power distribution board using the appropriate wiring harness or cables. Ensure that all necessary connections are securely made.

Firmware: ArduPlane/ArduCopter: Flash the desired ArduPlane or ArduCopter firmware onto the Cube Orange+ flight controller. 


PS: Here3+: Connect the Here3+ GPS module to the Cube Orange+ flight controller. Usually, this is done using a UART or I2C interface.


Telemetry RFD900: Connect the RFD900 telemetry module to both the Cube Orange+ flight controller and your ground control station (GCS) or ground telemetry device. This can typically be achieved using UART or Serial connections. Again, consult the RFD900 documentation for the specific pinout and wiring requirements.


On-board computer: Jetson Nano: Connect the Jetson Nano to the Cube Orange+ flight controller and power it using the appropriate power supply or battery. Utilize a suitable communication protocol (such as UART, USB, or Ethernet) to establish a connection between the Jetson Nano and the flight controller. 
 
5GHz RF: connect via I2C interface a 5GHz RF module and an antenna
