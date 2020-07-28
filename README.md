# QiskitTutorial

Basic Qiskit tutorials prepared for the DESY workshop on quantum computing. Content will be added shortly before the tutorial.

## Prerequisites
[Qiskit](https://github.com/Qiskit/qiskit "Qiskit") requires Python 3.5 or later. If you do not have Python, we recommend installing [Anaconda](https://www.anaconda.com/products/individual "Anaconda Individual Edition").

To separate Qiskit from existing Python packages, we recommend setting up a virtual environment. If you are using Anaconda, you can follow the instructions [here](https://qiskit.org/documentation/install.html "Qiskit Installation Instructions"). If you are using pip, instructions how to create a virtual environment can be found [here](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/).
After creating a new environment, activate it and make sure you have the latest version of pip. To do so run 

```
pip install --upgrade pip
```

Afterwards install the Qiskit package via

```
pip install qiskit
pip install qiskit[visualization]
```

(if you are using zsh, the last part needs to be in quotes).

Throughout the tutorial we will work with [Jupyter Notebooks](https://jupyter.org/ "Jupyter") which can be installed via 

```
conda install -c conda-forge jupyterlab
```

in case you are using Anaconda, or via 

```
pip install jupyterlab
```

in case you do not use Anaconda.

## Testing your Qiskit installation

To check if the installation was successful, you can now start a Python prompt or a Jupyter notebook and run the following commands

```Python
import qiskit
qiskit.__qiskit_version__
```

This should display a dictionary containing the version numbers of every part of the Qiskit SDK.


## Authors

* [**Stefan Kühn**](https://github.com/kuehnste)