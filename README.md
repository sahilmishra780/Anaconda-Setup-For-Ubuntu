# Setup Anaconda, Jupyter Notebook, Virtual Environments (conda) for Ubuntu 19.10
Install Anaconda from the anaconda website.<br><br>
During the installation the installer prompts “Do you wish the installer to initialize Anaconda3 by running conda init?”. Check yes at this prompt.<br><br>
Check installation by running ``anaconda-navigator``. 

If this command is not recognized, add the line ``export PATH=/home/yourUserName/anaconda3/bin:$PATH`` to the ``~/.bashrc`` file. Source the bash file by ``source ~/.bashrc`` or close the terminal and reopen a new terminal.<br><br>
To control whether or not each shell session has the base environment activated or not, run ``conda config --set auto_activate_base False or True``. To run conda from anywhere without having the base environment activated by default, use ``conda config --set auto_activate_base False``. This only works if you have run ``conda init`` first.<br><br>
Create a new conda environment variable by ``conda create -n myenv``. Activate this environment by ``conda activate myenv``. Launch jupyter notebook by running ``jupyter-notebook``. If you click new you may not see the newly created environment variable ``myenv``. <br><br>
To see the environenment variables activated and in the list of enviroment variables in the jupyter-notebook session, run the following in the ``base`` enviroment,<br>
``conda install nb_conda_kernels``<br>
``conda install nb_conda``<br>
``conda install ipykernel``<br><br>
Now activate ``myenv`` and install ``nb_conda_kernels`` for ``myenv`` by running,<br>
``conda activate myenv``<br>
``conda install nb_conda_kernels``<br><br>
With the ``myenv`` activated run ``jupyter-notebook``. You should now see the ``myenv`` environment variable activated when you click new. <br><br>
For more info refer to https://stackoverflow.com/questions/39604271/conda-environments-not-showing-up-in-jupyter-notebook

