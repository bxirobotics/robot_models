# Introduction
Description files of [`BXI robots`](https://bxirobotics.com/).     
Both URDF & MJCF files are prepared.

## Robots:
* [`Elf2 with 25 DOF`](https://github.com/bxirobotics/robot_models/tree/main/elf2_dof25)
* [`Elf2 with 12 DOF(rest are locked)`](https://github.com/bxirobotics/robot_models/tree/main/elf2_dof12)


## Gallery
<p float="left">
  <img src="elf2_dof25/xml/elf2_dof25.png" width="400">
</p>


# Usage | Display Robot Description
## Display Model 
MJCF file, with Mojuco py:
```
python -m mujoco.viewer --mjcf path/to/robot_models/elf2_dof25/xml/scene.xml     
```
URDF file, with [yourdfpy](https://github.com/clemense/yourdfpy):
```
yourdfpy  path/to/robot_models/elf2_dof25/urdf/elf2_dof25.urdf    
```
## Use Model Files    
Import model files as python submodule with [robot_descriptions.py](https://github.com/robot-descriptions/robot_descriptions.py)   

Please refer to robot_descriptions.py docs.    
Show description:
```
pip install robot_descriptions
ython -m robot_descriptions show_in_meshcat elf2_description  
```

