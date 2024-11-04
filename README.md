# DL-7643-Proj-Stuff
Project materials for CS 7643 Deep Learning Fall 2024, Georgia Tech


Dataset (Subset): https://huggingface.co/datasets/richidubey/Mini-KAIST-Multispectral-Pedestrian-Detection-Dataset
Dataset (Actual): https://huggingface.co/datasets/richidubey/KAIST-Multispectral-Pedestrian-Detection-Dataset

## Accesing GPUs via pace:
`ssh rdubey36@login-ice.pace.gatech.edu -L 8888:localhost:8888`  

Only run the first time that you access pace. 
(Used to link conda env to scratch directory which has a much larger storage quota.)
(Can use pace-quota to check your quota)
`mkdir ./scratch/.conda`
`ln -s ~/scratch/.conda ~/.conda`

`salloc --nodes=1 --gres=gpu:A100 -t5:00:00 --ntasks-per-node=24`    
`# requests a single A100 gpu and 24 cpu cores`    
`# Can request for H100 too, which is better.`    

`nvidia-smi #See GPU usage`    

`ml anaconda3 #Set up modules`    

`#cd to your directory and run`    

`jupyter notebook --ip 0.0.0.0`    

Now open vscode locally and ssh-connect to rdubey36@login-ice.pace.gatech.edu and use the kernel that jupter notebook command
above provided.