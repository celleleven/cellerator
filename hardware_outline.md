



# Hardware Outline

*TL/DR*: Cellerator is structured off the anatomy and physiology of a human.  The electrical supply is compared to heart, and data is comapred the the nervous system.  

Cellerator's brain is based off a single board computer (SBC) currently a Raspberry Pi.  The Raspberry Pi has two types of data; implicit and explicit.  Implicit data is the operating system, and the commands used to interaction with the physical world located on the SD Card.  The explicit data is the long-term memory stored chronologically. This data can be images, movies, data points, processed data, and results.  All long term data is stored in the external hard drive. The brain communicates with the Motor cortex (Arduino Uno).  The Arduino Uno control is responsible for planning, control and execution of voluntary movement in the form of G-code.   




```
Brain (Raspberry Pi)
  |   | -> Optic Nerve (HDMI -> 8MP Camera) 
  V   | ->  
Motor Cortex -> Arduino Uno
  |
  V
CNS -> CNC Shield
  |
  V


```

```
+------


                                +---------+            +---------+
[ Raspberry Pi ] -> CSI <------ |Arducam  | <--HDMI--> |Arducam  | <---- 8 MP Camera
               | -> GPIO 15 <-> | extender|            | extender| -----> SG90 Servo
               | -> GROUND ---> |         |            |         | --|
               \ -> 5VDC -----> |         |            |         | --/
                                +---------+            +---------+



```
