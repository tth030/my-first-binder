# my-first-binder
my-first-binder

This repository contains a collection of Jupyter notebooks that contains the display and the analysis of data presented in the following research paper:


- [How to run the notebooks?](#how-to-run-the-notebooks)
    - [Run in the cloud (Binder)](#run-in-the-cloud-binder)
    - [Install and run locally (Conda)](#install-and-run-locally-conda)
- [How to contribute?](#how-to-contribute)

## How to run the notebooks?

### Run in the cloud (Binder)

You can run the notebooks in your browser without installing anything thanks to
[binder](https://mybinder.org/). Just follow the link below or click on the
"launch binder" badge above and it will launch remotely a new notebook server
for you:

- [Run on binder](https://mybinder.org/v2/gh/tth030/my-first-binder/main?labpath=start.ipynb)

### Install and run locally (Conda)

Assuming that you have `git` and [conda](https://conda.io/docs/index.html)
installed, you can install all the packages required to run the notebooks in a
new conda environment using the following commands:

```bash
$ git clone https://github.com/fastscape-lem/fastscape-demo
$ cd fastscape-demo
$ conda env create -f environment.yml
$ conda activate SM_ESR_isostasy
```

You also need to install a few Jupyterlab extensions with the following command
(this step won't be required anymore with Jupyterlab >= 3.x):

```bash
$ jupyter labextension install \
    @jupyter-widgets/jupyterlab-manager \
    @pyviz/jupyterlab_pyviz \
    dask-labextension \
    ipygany
```

Finally run the command below to start the Jupyterlab application. It should
open a new tab in your browser.

```bash
$ jupyter lab
```
