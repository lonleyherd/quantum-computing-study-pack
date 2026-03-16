# Quantum Computing Basics

## What It Is

Quantum computing is a way of computing that uses quantum systems instead of ordinary bits. A classical bit is either `0` or `1`. A quantum bit, or `qubit`, can be in a combination of `0` and `1` until it is measured.

Quantum computers are not general replacements for classical computers. Their promise is in a smaller set of problems where quantum effects can be used to shape probabilities in useful ways.

## Three Core Ideas

### 1. Superposition

A qubit can exist in a blend of `0` and `1`. This does not mean we see both answers directly. It means the qubit has a quantum state that can later produce either result when measured.

Analogy: think of a spinning coin. While spinning, it is not simply heads or tails in the same practical sense as a coin lying flat. A qubit is more subtle than that analogy, but it helps build intuition.

### 2. Entanglement

Two or more qubits can become linked so their states must be described together. When qubits are entangled, you cannot fully explain one qubit without considering the others.

Entanglement is one of the main reasons quantum systems can behave in ways classical systems cannot easily copy.

### 3. Interference

Quantum algorithms work by increasing the likelihood of useful outcomes and decreasing the likelihood of unhelpful ones. This is called interference.

This is the key correction to a common myth: quantum computers do not simply "try every answer at once." Their power comes from carefully designed operations that make some answers more likely when measured.

## How a Quantum Program Works

A quantum program is usually written as a circuit:

1. Start qubits in a known state.
2. Apply gates to change or entangle the qubits.
3. Measure the qubits to get classical bits out.

Common gate examples:

- `X` gate: similar to flipping `0` to `1`
- `H` or Hadamard gate: creates superposition
- `CNOT` gate: entangles two qubits in many common circuits

## Worked Example

Start with one qubit in the state `|0>`.

Apply a Hadamard gate:

- the qubit moves into an even superposition of `|0>` and `|1>`
- if you measure right away, you will get `0` about half the time and `1` about half the time

That sounds simple, but the real power appears when several gates are chained together before measurement. Then the amplitudes can interfere, making some results more likely than others.

## Why People Care

Quantum computers may become useful for:

- simulating molecules and materials
- some optimization problems
- parts of cryptography and cryptanalysis
- certain linear algebra and search-style problems

Today, quantum hardware is still noisy and limited. That means current devices make errors easily and cannot yet solve most practical problems better than classical machines.

## Key Terms

- `Qubit`: the quantum version of a bit
- `Circuit`: a sequence of quantum gates and measurements
- `Gate`: an operation that changes the state of qubits
- `Measurement`: converting a qubit state into a classical result
- `Bloch sphere`: a visual model for a single qubit state
- `Noise`: physical errors that disturb the quantum system

## Advanced Caveat

The phrase `a|0> + b|1>` is shorthand for a quantum state with complex amplitudes. Those amplitudes are not ordinary probabilities, but their squared magnitudes determine measurement probabilities.

That is why quantum computing feels unfamiliar at first: the internal math is about amplitudes, while the final outputs are ordinary measured probabilities.

## Next Steps

Study these next, in order:

1. single-qubit gates like `X`, `Z`, and `H`
2. the Bloch sphere
3. Bell states and entanglement
4. simple algorithms like Deutsch-Jozsa and Grover's algorithm
