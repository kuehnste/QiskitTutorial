# QiskitTutorial

Basic Qiskit tutorials prepared for the quantum computing block course at RWTH.

## Running Qiskit

For the tutorials we are going to use [Qiskit](https://github.com/Qiskit/qiskit "Qiskit"). There are two options to work with Qiskit. The first one is to install it locally on your machine. The second option is to obtain an IBMQ account for IBM's quantum experience and use the IBM Quantum Lab to run the notebooks. Both options are described below.

### Prerequisites for running locally and installation instructions
[Qiskit](https://github.com/Qiskit/qiskit "Qiskit") requires Python 3.6 or later. If you do not have Python, we recommend installing [Anaconda](https://www.anaconda.com/products/individual "Anaconda Individual Edition").

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

### Testing your localQiskit installation

To check if the installation was successful, you can now start a Python prompt or a Jupyter notebook and run the following commands

```Python
import qiskit
qiskit.__qiskit_version__
```

This should display a dictionary containing the version numbers of every part of the Qiskit SDK.

### Obtaining an account for IBM Quantum Experience 

If you would like use IBM Quantum Lab or to run on IBM's quantum systems, you have to create an IBM Quantum Experience Account first. The account can be obtained [here](https://quantum-computing.ibm.com/login "IBM Quantum Experience"). 

To use IBM Quantum Lab log into your account, locate the IBMQ Quantum Lab on your dashborad and click on "Launch Lab".

## Using IBM's quantum hardware

After obtaining an IBM Quantum Experience Account follow the instructions [here](https://quantum-computing.ibm.com/lab/docs/iql/manage/account/ibmq "Saving the API token") to store your API token machine. Afterwards you can access the openly available quantum devices as described on the website.

## Authors

* [**Stefan Kühn**](https://github.com/kuehnste)