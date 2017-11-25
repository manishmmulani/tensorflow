# tensorflow

Download anaconda3 for python3.6

conda create -name tensorflow python=3.6

source activate tensorflow

tensorflow> pip install https://storage.googleapis.com/tensorflow/linux/cpu/tensorflow-1.4.0-cp36-cp36m-linux_x86_64.whl

tensorflow> python

python> import tensorflow as tf

python> tf.__version__

tensorflow> jupyter notebook

git clone https://github.com/PAIR-code/facets.git

jupyter nbextensions install facets-dist/ --user


# No module named 'error'

tensorflow> jupyter --paths

you will see that in /usr/local/share/jupyter/kernels/ directory contains only python2

Hence to install ipykernel for python3, run the following commands


sudo /home/mulani/installations/anaconda3/bin/python -m pip install ipykernel

sudo /home/mulani/installations/anaconda3/bin/python -m ipykernel install

(Ref https://github.com/jupyter/notebook/issues/1524 for the above)

Also, had to fix the python path in jupyter kernel as below

tensorflow>sudo vim /home/mulani/installations/anaconda3/share/jupyter/kernels/python3/kernel.json

"/home/mulani/.conda/envs/tensorflow/bin/python"
