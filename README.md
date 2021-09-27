# QOSF-mentorship-program
This repository contains code for a partial solution to task1 of cohort 4 screening tasks for the QOSF mentorship program

There are 3 ipynb files in the repository

## qRAM.ipynb
The qram has two qubit address as input and one qubit output

### Storing in qRAM
If at a position in input array the number satisfies the stated conditions then at that address in qram ,1| will be stored

### Querying the qRAM
Input address to qram will produce output <1| if at that address in the qram <1| is stored

![qRAM circuit](/Images/qRAM.png)

## Oracle.ipynb
This program implements the oracle circuit of the Grover's algorithm

### Working of oracle
The oracle has 4 qubits as input and 2 qubits as output

Two input qubits are control qubits and they always have same value

If the control qubits are 1 then phase of the 2 qubit state is flipped

If the control qubits are 0 then phase of the 2 qubit state is not flipped

![Oracle circuit](/Images/oracle.png)

## Diffuser.ipynb
This program implements the diffuser circuit of the Grover's algorithm

The output of diffuser is rotation of input state about the starting state of algorithm

![Diffuser circuit](/Images/diffuser.png)

## Circuit.ipynb
This program combines the qram, oracle and diffuser circuit.

Following are the steps in circuit.ipynb
1. Create equal superposition of 2 qubit states
2. Load <0| or <1| in qram according to input array
3. Pass the equal superposition and output of qram throgh the oracle of grover's algorithm
4. Pass the output of oracle throgh a diffuser. 


## Block diagram of circuit
![block diagram of circuit](/Images/complete_circuit.jpeg)
