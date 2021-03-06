Codes for conference paper ["A novel DDPG method with prioritized experience replay"](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8122622)

### Demo videos
The following videos record the performance of our trained model running on five tasks in the OpenAI gym:

![demo1](https://github.com/cardwing/Codes-for-RL-PER/blob/master/demo_gif/inverted_pendulum.gif) 
![demo1](https://github.com/cardwing/Codes-for-RL-PER/blob/master/demo_gif/inverted_double_pendulum.gif)
![demo1](https://github.com/cardwing/Codes-for-RL-PER/blob/master/demo_gif/hopper.gif)
![demo1](https://github.com/cardwing/Codes-for-RL-PER/blob/master/demo_gif/halfcheetah.gif)
![demo1](https://github.com/cardwing/Codes-for-RL-PER/blob/master/demo_gif/walker.gif)

### Requirements

- Tensorflow 1.4.0
- MuJoCo 
- Gym 0.7.4

### Install necessary components
    conda create -n tensorflow_gpu pip python=2.7
    source activate tensorflow_gpu
    pip install --upgrade tensorflow-gpu==1.4
    pip install gym==0.7.4
    pip install mujoco-py==0.5.5
    
    
### Run the code
    source activate tensorflow_gpu
    cd PER-in-RL
    CUDA_VISIBLE_DEVICES=0 python run_ddpg_mujoco.py

### Notes
    export MUJOCO_PY_MJKEY_PATH=/path/to/mjpro131/bin/mjkey.txt
    export MUJOCO_PY_MJPRO_PATH=/path/to/mjpro131

You need to have the above mujoco key file in your path. Now, you can reproduce the results in our paper.

### Cite RL-PER
```
@inproceedings{hou2017novel,
  title={A novel DDPG method with prioritized experience replay},
  author={Hou, Yuenan and Liu, Lifeng and Wei, Qing and Xu, Xudong and Chen, Chunlin},
  booktitle={Systems, Man, and Cybernetics (SMC), 2017 IEEE International Conference on},
  pages={316--321},
  year={2017},
  organization={IEEE}
}
```

### Acknowledgement
This repo is built upon [Tensorflow-Reinforce](https://github.com/yukezhu/tensorflow-reinforce) and [prioritized-experience-replay](https://github.com/Damcy/prioritized-experience-replay)

### Contact
If you have any problems in reproducing the results, just raise an issue in this repo.
