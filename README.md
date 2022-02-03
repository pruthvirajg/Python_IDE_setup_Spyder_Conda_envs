# Python_IDE_setup_Spyder_Conda_envs
Using Conda Python Environments with Spyder IDE 


## 1. Creating new environment with using anaconda cmd window
> Check the available environments
`conda env list`

> To create an new environment:
`conda create -n env_name`

or with python version
`conda create -n env_name python=3.7.4`

> To activate the environment, type
`conda activate env_name`

> To deactivate the environment (no need for env_name)
`conda deactivate`

> To delete an environment
`conda remove -n env_name --all`


## 2. Use the environment created in cmd window into spyder

> Install the SPyder kernel in the previous command window by activating the preious environment
> 
  `conda install spyder-kernels=2.1`
  
> To get the path of the Previously created  environment - step 2.1
>
`python -c “import sys; print(sys.executable)”`

> > Change the python interpreter in the below path of Spyder, Open Tools -> preferences

> select the “Use the following Python interpreter:” and paste the path as below and click Apply and OK

> To check if environment is activated
`import sys`

`print(sys.executable)`

## Jupyter

> To set the conda environment for jupyter,

First we have to install kernel
install ipykernel inside the environment with following cmd
`conda install -c anaconda ipykernel`

> check the installed kernel specs with the following cmd
`python -m ipykernel install --user --name=env_name`







https://medium.com/@apremgeorge/using-conda-python-environments-with-spyder-ide-and-jupyter-notebooks-in-windows-4e0a905aaac5
