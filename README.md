# Teaching Quantum Computing

Python notebooks I use to teach quantum computing and quantum key distribution. They start with the Python needed for the course, move through circuits and density matrices, and end with full simulations of the BB84, B92 and E91 protocols, including what an eavesdropper does to the key.

Each notebook opens in Google Colab and installs what it needs in its first cell.

## Modules

| Order | Notebook | What it covers |
|---|---|---|
| 1 | [`IntroPython.ipynb`](IntroPython.ipynb) | Python, NumPy, SymPy and Matplotlib basics, with a first look at the CHSH inequality. |
| 2 | [`QI_tools.ipynb`](QI_tools.ipynb) | Building and simulating circuits in Cirq and Qiskit: single-qubit gates, CNOT, Bell states, statevectors, measurement and histograms on the Aer simulator. |
| 3 | [`DensityMatrix.ipynb`](DensityMatrix.ipynb) | Pauli matrices and rotations in SymPy, tensor products, density matrices for pure and mixed states, Bloch vectors, purity and partial traces. |
| 4 | [`QKD.ipynb`](QKD.ipynb) | B92 and BB84 key distribution with and without an eavesdropper, the CHSH inequality and its violation by a Bell state, and the entanglement-based E91 protocol. |
| 5 | [`BB84.ipynb`](BB84.ipynb) | A complete BB84 pipeline: encoding, eavesdropping, decoding and key matching, followed by Cascade error correction and a look at classical Diffie-Hellman key exchange and why a quantum computer threatens it. |

## Running locally

```bash
pip install qiskit qiskit-aer cirq sympy numpy matplotlib pylatexenc
jupyter notebook
```

## License

Released under the [MIT License](LICENSE). Questions are welcome at syed.shubha@ieee.org.
