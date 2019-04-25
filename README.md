# Setting up the development environment
1.	Ubuntu on Windows (skip if you have an UNIX operating system)
-Enable Windows Subsystem for Linux
-Download Ubuntu from the Microsoft Store
2.	Set up Python3 and pip
-CMD: sudo apt-get install python3 python3-pip
3.	Jupyter, virtualenv and ipykernel
-CMD: pyton3-pip install jupyter virtualenv
-Setting up virtualenv & making it available in jupyter
    i.	CMD: Python3 –m virtualenv CartPole
    ii.	CMD: source CartPole/bin/activate
    iii.	CMD: Pip install ipykernel
    iv.	CMD: Python –m ipykernel install --user --name=CartPole
4.	Set up Jupyter Notebook
-CMD: Jupyter notebook
-Create new Notebook in the pop-up window (see figure 6).

Note: If the window does not show go to localhost:8888 in your browser

# Visualizing environments
Visualizing the environments is a nice addition to the notebook, but not really important for the research.
But in short: it is done using an Xvfb server and the IPython and Pillow libraries, which can be seen in the create_gif method.

XVFB is necessary which can be installed with sudo apt-get install xvfb
Also use: “xvfb-run -s "-screen 0 1400x900x24" jupyter notebook” to run jupyter, to be able to render.
