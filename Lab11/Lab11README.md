# Lab 11: Qiskit Installation and Bell State Execution

This lab walks through the installation and setup of Qiskit on an Ubuntu system, as well as running a Bell state example using the Aer simulator. The goal was to verify quantum entanglement using Qiskit's `QuantumCircuit` and simulate results using `aer_simulator`.

---

## Step 1: Update and Install Python Pip + Virtual Environment

We start by updating system packages and installing `python3-pip` and `python3-venv`. These are required to create an isolated Python environment for Qiskit installation.

![step1](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab11/lab11%231.png?raw=true)

---

## Step 2: Create and Activate Virtual Environment

A new virtual environment named `qiskit-env` is created and activated using Python 3. This ensures no conflict with system-level Python packages.

```bash
python3 -m venv qiskit-env
source qiskit-env/bin/activate
```

Then we proceed with installing Qiskit visualization tools.

![step2](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab11/lab11%232.png?raw=true)

---

## Step 3: Install Qiskit-Aer and Qiskit IBM Provider

`qiskit-aer` is installed to support local simulation of quantum circuits. `qiskit-ibm-provider` is used to access IBM Quantum backends. These are essential for the lab.

![step3](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab11/lab11%233.png?raw=true)

---

## Step 4: Load IBM Provider and Verify Backends

We import `IBMProvider`, initialize it, and verify the available IBM backends. This confirms that the API key was saved correctly and communication with IBM Quantum systems is active.

```python
from qiskit_ibm_provider import IBMProvider
provider = IBMProvider()
print(provider.backends())
```

![step4](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab11/lab11%234.png?raw=true)

---

## Step 5: Bell State Python Code

We write a Python script (`bell_example.py`) that sets up a Bell state circuit using Qiskit. The circuit uses a Hadamard gate followed by a CNOT to entangle two qubits.

```python
from qiskit import QuantumCircuit, transpile
from qiskit_aer import Aer

backend = Aer.get_backend("aer_simulator")

qc = QuantumCircuit(2)
qc.h(0)
qc.cx(0, 1)
qc.measure_all()

compiled = transpile(qc, backend)
result = backend.run(compiled).result()
print("Result:", result.get_counts())
```

This code is entered using `nano bell_example.py`.

![step5](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab11/lab11%235.png?raw=true)

---

## Step 6: Run Bell State Simulation

We run the Bell state script, and as expected, the measurement results show roughly equal distribution between `00` and `11`, confirming entanglement.

```bash
python bell_example.py
```

Result:

```text
Result: {'11': 534, '00': 490}
```

![step6](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab11/lab11%236.png?raw=true)

---

## Summary

This lab demonstrates how to:

- Install and configure Qiskit in a virtual environment on Ubuntu
- Use Qiskit Aer to simulate quantum circuits
- Run and observe quantum entanglement using a Bell state example

We successfully verified quantum behavior through reproducible simulation results and established connection to IBM Quantum backends.

