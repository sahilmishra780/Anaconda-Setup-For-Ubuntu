# Setup Anaconda, Jupyter Notebook, Virtual Environments (conda) for Ubuntu 19.10
Install Anaconda from the anaconda website.<br><br>
During the installation the installer prompts “Do you wish the installer to initialize Anaconda3 by running conda init?”. Check yes at this prompt.<br><br>
Check installation by running ``anaconda-navigator``. If this command is not recognized, append the ``~/.bashrc`` with ``export PATH=/home/yourUserName/anaconda3/bin:$PATH``. Source the bash file by ``source ~/.bashrc`` or close the terminal and reopen a new terminal.<br><br>
To control whether or not each shell session has the base environment activated or not, run ``conda config --set auto_activate_base False or True``. To run conda from anywhere without having the base environment activated by default, use ``conda config --set auto_activate_base False``. This only works if you have run ``conda init`` first.

