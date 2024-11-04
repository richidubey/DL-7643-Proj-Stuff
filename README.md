# DL-7643-Proj-Stuff
Project materials for CS 7643 Deep Learning Fall 2024, Georgia Tech


Dataset: https://huggingface.co/datasets/richidubey/KAIST-Multispectral-Pedestrian-Detection-Dataset

**Accesing GPUs via pace:**
ssh rdubey36@login-ice.pace.gatech.edu -L 8888:localhost:8888
salloc --nodes=1 --gres=gpu:A100 -t5:00:00 --ntasks-per-node=24
# requests a single A100 gpu and 24 cpu cores
# Can request for H100 too, which is better.


nvidia-smi #See GPU usage

ml anaconda3 #Set up modules

#cd to your directory and run

jupyter notebook --ip 0.0.0.0

#Now open vscode locally and ssh-connect to rdubey36@login-ice.pace.gatech.edu and use the kernel that jupter notebook command
above provided.