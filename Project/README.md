
# RL Project for Coursework 2020
## MolDQN-pytorch

PyTorch implementation of MolDQN as described in [Optimization of Molecules via Deep Reinforcement Learning](https://www.nature.com/articles/s41598-019-47148-x)
by Zhenpeng Zhou, Steven Kearnes, Li Li, Richard N. Zare and Patrick Riley.

## Installation

## <a name="source"></a>From source:

1) Install `rdkit`.  
   `conda create -c rdkit -n my-rdkit-env rdkit`  
   `conda activate my-rdkit-env`  
   `conda install -c conda-forge rdkit`  
   
2) Clone this repository.  
   `git clone https://github.com/aksub99/MolDQN-pytorch.git`  
   `cd MolDQN-pytorch`
   
3) Install the requirements given in `requirements.txt`.  
   `pip install -r requirements.txt`  
   
4) Install `baselines`.  
   `pip install "git+https://github.com/openai/baselines.git@master#egg=baselines-0.1.6"`  
   
Please remember to modify the `TB_LOG_PATH` variable in `main.py` depending on where you wish to store your tensorboard runs file.
## Training the MolDQN:

`python main.py`

A simple example to train the model on a single property optimization task can be seen in `Moldqn_implementation.ipynb`.

## Results:

#### Simulated Results available in the pdf.[RL_Project_Results.pdf](https://github.com/Ghanendra19213/Ghanendra_MT19213_RL_M2020/blob/master/Project/RL_Project_Results.pdf).
#### The following was the reward curve obtained when the model was trained for 5000 episodes on a single property optimization task (QED in this case).

<img src="https://github.com/Ghanendra19213/Ghanendra_MT19213_RL_M2020/blob/master/Project/Tensorboard_Results.PNG">
