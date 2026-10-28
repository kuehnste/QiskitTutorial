# QiskitTutorial

Basic tutorials on quantum computing with Qiskit, prepared for the Quantum Computing Block Course at RWTH Aachen University.


## Running Qiskit

The tutorials use [Qiskit](https://github.com/Qiskit/qiskit "Qiskit"), an open-source SDK for quantum computing. To work through the notebooks you have to install Qiskit and Jupyter on your computer

### Prerequisites 
[Qiskit](https://github.com/Qiskit/qiskit "Qiskit") requires Python 3.10 or later.  requires Python 3.10 or later. If Python is not installed on your computer, download the latest stable version from the [official Python website](https://www.python.org/downloads/).

We recommend using a virtual environment to keep the dependencies for these tutorials separate from other Python projects. For instructions on creating and activating a virtual environment, see the [Python Packaging User Guide](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/).


### Installation

After creating and activating your virtual environment, upgrade `pip` to the latest version:

```Bash
pip install --upgrade pip
```

Next, install Qiskit and its visualization dependencies:

```Bash
pip install qiskit
pip install qiskit[visualization]
```

**Note**: Quotation marks around `'qiskit[visualization]'` are necessary when using the Zsh shell. 

We also recommend installing Qiskit Aer, a simulator that allows you to run quantum circuits on your local computer without using quantum hardware:

```
pip install qiskit-aer
```

Throughout the tutorial we will work with [Jupyter Notebooks](https://jupyter.org/ "Jupyter") which can be installed via 

```Bash
pip install jupyterlab
pip install notebook
```

### Running Notebooks

To start JupyterLab, run the following command in your terminal:
```Bash
jupyter lab
```

Alternatively, you can launch the classic Jupyter Notebook interface:
```Bash
jupyter notebook
```
Open the relevant tutorial notebook (.ipynb file) in the interface to get started.

### Verifying your local Qiskit installation

To check that Qiskit is installed correctly, open a Python interpreter or a Jupyter notebook and run:
```Python
import qiskit
qiskit.__qiskit_version__
```

This should display a dictionary containing the version numbers of every part of the Qiskit SDK.

You can also check whether Qiskit Aer is available:
```Python
import qiskit_aer
print(qiskit_aer.__version__)
```

If both commands execute without errors, the corresponding packages are installed and ready to use.

### Obtaining an account for IBM Quantum Experience 

If you would like use IBM Quantum Lab or to run on IBM's quantum systems, you have to create an IBM Quantum Experience Account first. The account can be obtained [here](https://quantum.cloud.ibm.com/signin "IBM Quantum Experience"). 

## Using IBM's quantum hardware

After obtaining an IBM Quantum Experience Account follow the instructions [here](https://quantum.cloud.ibm.com/docs/en/guides/hello-world "Getting ready to run on hardware"). Afterwards you can access the openly available quantum devices as described on the website.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Authors

[**Stefan Kühn**](https://github.com/kuehnste)

