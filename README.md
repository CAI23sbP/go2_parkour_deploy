# Unitree GO2 Deploy

This repo is a Unitree GO2 Deployment which have been trained by IsaacLab.

We are supporting deployment in a Mujoco simulation and RealWorld.

### 1. Installation

`cd IsaacLab ## going to your IsaacLab folder`

`git clone https://github.com/CAI23sbP/go2_deploy.git`

`cd go2_deploy && pip3 install -e .`


### 2. How to use

`export LD_PRELOAD=/usr/lib/x86_64-linux-gnu/libstdc++.so.6`

`export LD_LIBRARY_PATH=~/anaconda3/envs/env_isaaclab/lib:$LD_LIBRARY_PATH`

### 3. Sim2Sim  

### 3.1. Create parkour_demo env 

`python3 mujoco_deploy/mujoco_terrain_generator.py`

![alt text](<Screenshot from 2025-09-08 19-42-46.png>)

### 3.2. Deploy mujoco

`python3 scripts/go2_deploy --interface lo`

<video controls src="Screencast from 2025년 09월 08일 19시 33분 34초.webm" title="Title"></video>


### 4. TODO list

* [ ] Make Real-world deployment code


### Acknowledgement

Thanks to their previous projects.

1. @machines-in-motion [repo](https://github.com/machines-in-motion/Go2Py)

2. @NVlabs [repo](https://github.com/NVlabs/HOVER)

3. @eureka-research [repo](https://github.com/eureka-research/eurekaverse)

4. @boston-dynamics [repo](https://github.com/boston-dynamics/spot-rl-example)

5. @itt-DLSLab [repo](https://github.com/iit-DLSLab/gym-quadruped)