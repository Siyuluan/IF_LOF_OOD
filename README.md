This repository contains our source code for the paper submission 
Siyu Luan, Zonghua Gu, Leonid Freidovich, Lili Jiang, Out-Of-Distribution Detection for Deep Neural Networks with Isolation Forest and Local Outlier Factor.
It is based on the open-source software provided by the authors of
Henzinger, Thomas A., Anna Lukina, and Christian Schilling. "Outside the box: Abstraction-based monitoring of neural networks." arXiv preprint arXiv:1911.09032 (2019).
We added Isolation Forest and Local Outlier Factor for runtime monitoring and anomaly/outlier detection of neural networks. 


## Models

The repository contains the pretrained models used in the evaluation.
The models can be recomputed using the scripts `run/train_INSTANCE.py` where `INSTANCE` is the name of the model/data combination.

## Evaluation

We only show our results. For faster calculation, some experiments of the original author are deleted here. If you want to reproduce it completely, please delete part of the python comment code

Here only take the GTSRB data set as an example



1. In the run/run_experiments file, you should change the path to your own path， and run this script

2 In the evaluate_all function, set True for LOF, False for IF

3 In the EvaluateCombination file, change the hyperparameters of IF or LOF by changing for loop

4 When the program ends, it will display Done! You should get the result txt now.

5 Results are in the file