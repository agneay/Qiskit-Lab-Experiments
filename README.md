# Quantum Computing Lab — 23CSE463

Worksheet 1 experiments on **Introduction to Bits, Gates and Quantum Circuits**, implemented in Qiskit as individual Jupyter notebooks.

**Name:** Agneay B Nair
**Register No.:** CH.SC.U4CSE24102
**Course:** 23CSE463 – Quantum Computing
**Date:** 18/06/2026

## Aim

To study the fundamental concepts of quantum computing — classical bits, qubits, quantum states, superposition, quantum gates, and quantum circuit representation — and to understand how quantum information is represented and manipulated using Qiskit.

## Contents

Each experiment is a separate, self-contained notebook with the aim, program task, code, and pre-run output (circuit diagrams, histograms, statevectors) already included.

| # | Notebook | Task |
|---|----------|------|
| 1 | `experiment_1_single_qubit_circuit.ipynb` | Create a quantum circuit with a single qubit and display the circuit diagram. |
| 2 | `experiment_2_pauli_x_gate.ipynb` | Apply the Pauli-X (NOT) gate on a qubit and observe the circuit. |
| 3 | `experiment_3_hadamard_superposition.ipynb` | Use the Hadamard gate to study the concept of superposition. |
| 4 | `experiment_4_two_qubit_cnot.ipynb` | Create a two-qubit circuit and apply a Controlled-NOT (CNOT) gate. |
| 5 | `experiment_5_bell_state.ipynb` | Construct a Bell State circuit using Hadamard and CNOT gates (entanglement). |
| 6 | `experiment_6_measure_single_qubit.ipynb` | Measure a single qubit and display the output. |
| 7 | `experiment_7_two_qubit_measurement.ipynb` | Create a two-qubit circuit and measure both qubits. |
| 8 | `experiment_8_x_h_cnot_circuit.ipynb` | Design and visualize a circuit containing X, H, and CNOT gates. |
| 9 | `experiment_9_aer_simulator_analysis.ipynb` | Simulate a circuit using the Aer Simulator and analyze the measurement results. |
| 10 | `experiment_10_classical_vs_quantum_bits.ipynb` | Compare the behavior of classical bits and quantum bits. |

Source material: `WORK SHEET 1 .docx` / `WORK SHEET 1 .pdf` in this folder.

## Requirements

- Python 3.10 or above
- [Qiskit](https://www.ibm.com/quantum/qiskit) and the Aer simulator
- Jupyter Notebook or VS Code
- Matplotlib and pylatexenc (for circuit diagrams)

## Setup

```bash
# Create and activate a virtual environment
python -m venv qiskit-env
qiskit-env\Scripts\activate        # Windows
# source qiskit-env/bin/activate   # macOS/Linux

# Upgrade pip
python -m pip install --upgrade pip

# Install dependencies
pip install qiskit qiskit-aer matplotlib pylatexenc notebook

# Verify installation
python -c "import qiskit; print(qiskit.__version__)"
```

## Running the notebooks

```bash
jupyter notebook
```

Then open any `experiment_*.ipynb` file and run all cells (**Cell → Run All**). Each notebook is independent, so they can be run in any order.

## Notes

- All notebooks were built and tested with Qiskit 2.x and `qiskit-aer` 0.17.x. Older Qiskit versions (< 1.0) use a different API (e.g. `qiskit.execute`, `qiskit.providers.aer`) and may require code changes.
- `AerSimulator` is used for all circuit simulations; no real quantum hardware or IBM Quantum account is required.
- Circuit diagrams use the `matplotlib` drawer (`qc.draw('mpl')`); the text drawer (`qc.draw()`) is also shown as a fallback.
