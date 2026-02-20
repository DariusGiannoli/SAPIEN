# Mujoco discovery and mac adaptation of the Berkeley Sim


## Provided Simulations: 
- biped_scene: only torso + legs
- full humanoid; legs + torso + arms (22 DoF)


### Run first: 
source .venv/bin/activate

export PYTHONPATH=".venv/lib/python3.10/site-packages:source/berkeley_humanoid_lite_lowlevel:source/berkeley_humanoid_lite"

### Run lower sim: 

mjpython scripts/sim2sim/play_mujoco.py --config ./configs/policy_biped_50hz.yaml

### Run Full Humanoid 

mjpython scripts/sim2sim/play_mujoco.py --config ./configs/policy_humanoid.yaml
