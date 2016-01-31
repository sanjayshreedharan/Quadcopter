# Quadcopter
An Indigenous Low cost Autopilot System for a Quadcopter using Arduino UNO

This project endeavours to design a low cost indigenous auto-pilot system for a quadcopter using the Arduino UNO. This tutorial majorly deals only with the design and deployment of the autopilot system and we assume that you already have the frame, motors, ESC’s and the power supply in place. Below is just a brief on getting the above setup ready. 

The frame can either be designed or it can be bought. For speedy development, I would suggest to go with buying a frame since frame design and construction takes a lot of time. A good frame to consider buying  would be Hobbyking X525 Glass Fiber Quadcopter Frame.

http://www.hobbyking.com/hobbyking/store/__22800__Hobbyking_X525_V3_Glass_Fiber_Quadcopter_Frame_600mm.html

We designed our own frame and since frame design and construction as such is a huge task, I would follow up with a tutorial for those of you who wish to design your own frames. My frame design was somewhat similar to the frame in the below link.

After the frame is ready, the next would be to get the motors, ESC’s, propellers and the power supply in place.The rating of the motors, ESC’s and power supply depends on the size of the frame and the pay-load capacity of the quadcopter. So, check out for tutorials and get that as well ready.

For autopilot, a 9DOF IMU (Inertial measurements unit), which consists of an accelerometer, gyroscope and a magnetometer is required. For wireless communication, Bluetooth or RC would do the job. We used the Bluetooth as we would be able to keep a watch on the state of the quadcopter through the serial monitor and also send commands. If flying low-heights and debugging is your requirement, go with bluetooth. For those of you who wish to fly great heights, use a RC module. 

The MPU6050 (6 DOF IMU with accelerometer and gyroscope) and HMC5883L(Magnetometer) was combined to give the quadcopter 9 degrees of freedom. The HC-06 module was used as bluetooth.

A custom Arduino UNO shield was designed for the purpose of a quadcopter. The schematic and the board design is available. So, if you know know how to make a PCB, you can make the shield with the MPU6050, HMC5883L and HC-06 on it and it would fit perfectly on top of the UNO.  

If making PCB is not your piece of cake, I would suggest you to connect the sensors with jumper wires. Make sure the connections, that you have made are reliable, if they are not this might pose a serious problem when the quadcopter is on the go.

After this is done, download the code and fuse it into your Arduino UNO.
