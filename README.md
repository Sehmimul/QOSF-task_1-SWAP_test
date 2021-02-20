# QOSF-task_1-SWAP_test

## In this project I answered the 3 questions below:

The Swap test is a simple quantum circuit which, given two states, allows you to compute how much do they differ from each other.

PART 1 - Provide a variational (also called parametric) circuit which is able to generate the most general 1 qubit state. By most general 1 qubit state we mean that there exists a set of the parameters in the circuit such that any point in the Bloch sphere can be reached. Check that the circuit works correctly by showing that by varying randomly the parameters of your circuit you can reproduce correctly the Bloch sphere.

PART 2 - Use the circuit built in step 1) and, using the SWAP test, find the best choice of your parameters to reproduce a randomly generated quantum state made with 1 qubit.

PART 3 - Suppose you are given with a random state, made by N qubits, for which you only know that it is a product state and each of the qubits are in the state | 0 > or | 1>. By product state we mean that it can be written as the product of single qubit states, without the need to do any summation. For example, the state
|a> = |01>
Is a product state, while the state
|b> = |00> + |11>
Is not. Perform a qubit by qubit SWAP test to reconstruct the state. This part of the problem can be solved via a simple grid search.

# Description

### For part 1, I made a variational quantum circuit, by using parameters alpha and theta such that I can get any point in the Bloch Sphere.

### For Part 2, I managed to reproduce the parameters (alpha and theta) of the original state to an accuracy of 0.1 radians. I optimized the parameters of an unknown qubit to reproduce the parameters. I used the optimization method, dual annealing.

### For part 3, I managed to reproduce the quantum state made of n qubits by loopiing through all the n qubits. I could use qubit-by-qubit SWAP test as the quantum state is a product state and thus, the n qubits are not entangled with any other qubit of the state. 

# Other Information

### The code may take some time to run as as I iterate a number of times while optimizing. 

# Referemces

### The following links provided me useful motivation while doing the project:
### [1] https://en.wikipedia.org/wiki/Swap_test
### [2] https://en.wikipedia.org/wiki/Spherical_coordinate_system
