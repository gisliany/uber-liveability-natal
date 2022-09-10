# Project Overview

This repository holds the files to reproduce the results found in the article *"A composite indicator of liveability based on sociodemographic and Uber quality service dimensions: a data-driven approach"*.

The Uber Estimated Time of Arrival (ETA) data are available for the neighborhoods and Human Development Units (HDU). However, it is worth mentioning this data are already preprocessed, imputed, and grouped by spatial level to obtain the final means and standard deviations. The raw data are not available due to the rules of the Uber Terms of Use. 

## Environment Setup

Create a conda environment with ``environment.yml``:

```bash
conda env create --file environment.yml
```

To remove an environment in your terminal window run:

```bash
conda remove --name myenv --all
```

To list all available environments run:

```bash
conda env list
```

The pip ``requirements.txt`` file is also available and it is possible to install some dependencies by running:

```bash
pip install -r requirements.txt
```

## Reproduce the results

After the installation, navigate to the folder where your notebooks are located, and start Jupyter server in your terminal window:

```
jupyter notebook
```

You can also open the notebooks using Visual Studio Code, being recommended to install the extensions: ```Python```, ```Jupyter``` and ```Jupyter Notebook Renderers```.

After that, you will be able to manipulate and reproduce the results by running the jupyter notebooks ```eda.ipynb``` and ```indicator.ipynb```. In both notebooks, you can set the variable ```spatial_unit``` as *"neighborhood"* or *"hdu"* and run all cells to see the results.
