# A Comparative Study of Asexual and Sexual Brain Reproduction for Morphologically Evolving Robots
In the most extensive robot evolution systems, both the bodies and the brains of the robots undergo evolution and the brains of 'newborn' robots are also optimized by a learning process immediately after `birth'. This research is concerned with the brain evolution mechanism in such a system. In particular, we compare four options obtained by combining Asexual or Sexual brain reproduction with Darwinian or Lamarckian evolution mechanisms. We conduct experiments in a mujoco simulator based wrapper called Revolve2. The release version of Revolve2 used in this project is v0.3.6-beta1 (https://github.com/ci-group/revolve2/releases/tag/v0.3.6-beta1).


## Installation 
Steps to install:
``` 
1. clone https://github.com/ci-group/revolve2/releases/tag/v0.3.6-beta1
2. git clone https://github.com/onerachel/Asexual_vs_Sexual_Reproduction.git
3. cd Asexual_vs_Sexual_Reproduction
4. virtualenv -p=python3.8 .venv
5. source .venv/bin/activate
6. ./dev_requirements.sh  (comment out this line since we don't need to use isaacgym simulator # pip install -e ./runners/isaacgym[dev] && \)
``` 

## Run experiments 
To run experiments, e.g. darwinian_point_navigation:
``` 
python darwinian_evolution/optimize.py
``` 
To show the simulation, add --visualize: 
``` 
python darwinian_evolution/optimize.py --visualize
``` 
To restart from the last optimization checkpoint, add --from_checkpoint: 
``` 
python darwinian_evolution/optimize.py --from_checkpoint
``` 
To plot fitness:
``` 
python darwinian_evolution/plot_fitness.py
``` 
To check the best robot wrt the fitnees:
``` 
cd darwinian_evoluation
python rerun_best.py
```
To check the best robot wrt the fitnees and save the video:
``` 
cd darwinian_evoluation
python rerun_best.py -r <OUTPUT-DIR>
```
## Partial results
