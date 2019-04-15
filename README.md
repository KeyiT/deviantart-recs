# kaggle_competition_template
Template for Kaggle Projects

## Setup package
1. Setup a new python virtual environment:
```bash
conda create --name <env_name> python=3.6
source activate <env_name>
```
2. Under the root folder
```bash
pip install -r requirements
```
3. create data folder and download data
```bash
mkdir input/<competition_name>
cd input/<competition_name>
kaggle competitions download -c <competition_name>
cd ../../
```
4. create a folder for kernel, create and push a kernel
```bash
mkdir <kernel_name>
cd <kernel_name>
kaggle kernels init -p ./
# TODO: create a notebook and modify the kernel metadata
kaggle kernels push <use_name>/<kernel_name> ./
```

