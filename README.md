# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```python
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
pos = [[1,30],[2,40],[3,90]]
robot = getRobot()
robot.driveJoints (0,0,0,0,0,0)
delay(5)
for i in pos:
robot.Controller.moveJoint (i[0],i[1])
delay (5)
```
## Output
### 1. Generic Articulated Robot
![Screenshot (3)](https://github.com/Saravana-kumar369/Movement-of-Robot-Joints/assets/117925254/641708ce-1843-442e-ab31-01c623f32d72)


### 2. robot.driveJoints(0,0,0,0,0,0)
![Screenshot (9)](https://github.com/Saravana-kumar369/Movement-of-Robot-Joints/assets/117925254/82256cc0-90e4-4236-a0d7-a75b1ac7f541)


### 3. Movement of Joint1
![Screenshot (4)](https://github.com/Saravana-kumar369/Movement-of-Robot-Joints/assets/117925254/56c52411-eda5-4e2d-a6f7-8e415ce768a3)


### 3. Movement of Joint2
![Screenshot (10)](https://github.com/Saravana-kumar369/Movement-of-Robot-Joints/assets/117925254/5e8560b7-066e-4d8a-9cda-b2b385bbc7ce)


### 3. Movement of Joint3
![Screenshot (9)](https://github.com/Saravana-kumar369/Movement-of-Robot-Joints/assets/117925254/0397a671-9f98-4145-8939-1776e32f1efb)


## Result 
Thus the different robots joints are moved with the help of python list.


