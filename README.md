# SQcircuit-examples
[![license](https://img.shields.io/badge/license-New%20BSD-orange.svg)](https://opensource.org/licenses/BSD-3-Clause)

This repository demonstrates how to use [``SQcircuit``](https://github.com/stanfordLINQS/SQcircuit) to simulate superconducting circuits. On examples ranging from simple qubits to state-of-the-art circuits in the literature, we show how to easily reproduce the main results of papers with ``SQcircuit``. 

There are also a set of tutorial notebooks showing how to use ``SQcircuit`` to compute the gradient of circuit properties (eigenfrequencies, decoherence times, coupling operators, …) with respect to the values of circuit elements, and how to use this information to optimize circuits for target performance.

## Simulating qubits from the literature

* [Qubit protected by two Cooper-pair tunneling](examples/two_CPB.ipynb): [Smith2020](https://doi.org/10.1038/s41534-019-0231-2) designed a qubit that is protected by two-Cooper-pair tunneling. This notebook reproduces the energy spectrum of the paper for the circuit.

* [Kite Circuit](examples/kite.ipynb): [Smith2022](https://doi.org/10.1103/PhysRevX.12.021002) designed a superconducting circuit that magnifies quantum phase fluctuations with Cooper-pair pairing. This notebook reproduces the figures from the paper including energy spectrum, wavefunctions, and matrix elements.

* [Inductively Shunted Circuit](examples/inductively_shunted.ipynb): [Smith2016](https://doi.org/10.1103/PhysRevB.94.144507) explained how conventional methods and perturbation theory do not correctly diagonalize their highly anharmonic inductively-shunted qubits. This notebook demonstrates how ``SQcircuit`` can quickly compute the exact energy spectrum without needing to consider these details.

* [Zero-Pi Qubit](examples/zeropi_qubit.ipynb): This notebook calculates the energy spectrum and eigenfunctions of the zero-pi qubit from [Groszkowski2018](https://doi.org/10.1088/1367-2630/aab7cd).

* [Flux Qubit](examples/flux_qubit.ipynb): This notebook calculates the energy spectrum of the flux qubit from [Robertson2006](https://doi.org/10.1103/PhysRevB.73.174526).

## Calculating gradients and performing optimization

* [Calculating gradients](examples/calculating_gradients.ipynb): This notebook shows how to calculate gradients with ``SQcircuit``.

* [Performing optimization](examples/gradient_based_optimization.ipynb): This notebook uses SQcircuit and PyTorch to perform gradient descent optimization with a fluxonium to achieve a desired qubit frequency.

## Documentation
The documentation for ``SQcircuit`` is provided at [sqcircuit.org](https://sqcircuit.org).