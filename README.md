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

`python3 scripts/go2_deploy --interface lo`

### 4. Sim2Real

`python3 scripts/go2_deploy --interface {$your network_interface}`

### 5. TODO list

* [x] Make sim2sim deployment code
* [ ] Opening sim2sim deployment code
* [ ] Make sim2real deployment code
* [ ] Opening sim2real deployment code
