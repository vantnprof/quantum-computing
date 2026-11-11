---
title: Quantum Computing Course
site:
  hide_title_block: true
  hide_outline: true
---

::::::{div}
:class: hero

:::::{grid} 1 1 2 2

::::{div}
:class: hero-text

:::{div}
:class: hero-kicker
Qubits · Circuits · Algorithms
:::

:::{div}
:class: hero-title
Learn to think in *superposition*
:::

From $\ket{0}$ to Shor's algorithm on real quantum hardware: 17 lectures and 2 projects, built from first principles in Python.

{button}`Start learning → <lectures/00-linear-algebra/index.md>` {button}`Roadmap <#roadmap>`
::::

::::{div}
:class: qconsole

`>>> qc = QuantumCircuit(2)`

`>>> qc.h(0); qc.cx(0, 1)`

`>>> Statevector(qc)`

`|Φ⁺⟩ = (|00⟩ + |11⟩) / √2`
::::

:::::

::::::

(roadmap)=
## 🗺️ Roadmap

### 🧮 Phase 1 · Mathematical Foundations

The complex numbers, linear algebra and notation every quantum computation is built on.

::::{grid} 1 2 2 3
:class: roadmap-grid phase-1

:::{card} 🧮 00 · Complex Numbers & Linear Algebra
:link: lectures/00-linear-algebra/index.md

The vectors, matrices and complex amplitudes that quantum states are made of.
:::

:::{card} 📐 01 · Dirac Notation
:link: lectures/01-dirac-notation/index.md

Bras, kets and the language physicists use to write quantum states.
:::

:::{card} 🐍 02 · Python & NumPy for Quantum
:link: lectures/02-python-for-quantum/index.md

Set up your lab: simulate qubits with NumPy, then with Qiskit.
:::

::::

### ⚛️ Phase 2 · Qubits & Gates

Meet the qubit: superposition, gates, measurement and entanglement.

::::{grid} 1 2 2 4
:class: roadmap-grid phase-2

:::{card} 🌐 03 · Qubits & the Bloch Sphere
:link: lectures/03-qubits-bloch-sphere/index.md

One qubit, infinitely many states, and a sphere to picture them.
:::

:::{card} 🎛️ 04 · Single-Qubit Gates
:link: lectures/04-single-qubit-gates/index.md

X, Y, Z, H, S, T: rotations that steer a qubit around the sphere.
:::

:::{card} 🎲 05 · Measurement
:link: lectures/05-measurement/index.md

Where quantum meets classical: probabilities, collapse and the Born rule.
:::

:::{card} 🔗 06 · Multi-Qubit Systems & Entanglement
:link: lectures/06-entanglement/index.md

Tensor products, CNOT, Bell states and correlations Einstein called spooky.
:::

::::

### 🔗 Phase 3 · Circuits & Protocols

Wire qubits into circuits and use them to communicate in ways classical bits can't.

::::{grid} 1 2 2 3
:class: roadmap-grid phase-3

:::{card} 🧩 07 · Quantum Circuits with Qiskit
:link: lectures/07-quantum-circuits-qiskit/index.md

Draw, simulate and debug quantum circuits in code.
:::

:::{card} 📡 08 · Teleportation & Superdense Coding
:link: lectures/08-teleportation-superdense/index.md

Move a quantum state with two classical bits, or send two bits with one qubit.
:::

:::{card} 🔐 09 · No-Cloning & Quantum Key Distribution
:link: lectures/09-no-cloning-qkd/index.md

Why qubits can't be copied, and how that makes communication secure.
:::

::::

### 🧠 Phase 4 · Quantum Algorithms

Interference as a computational resource: from oracles to factoring.

::::{grid} 1 2 2 4
:class: roadmap-grid phase-4

:::{card} ⚖️ 10 · Deutsch–Jozsa & Bernstein–Vazirani
:link: lectures/10-deutsch-jozsa/index.md

Your first quantum speed-ups, powered by phase kickback.
:::

:::{card} 🔎 11 · Grover's Search
:link: lectures/11-grover-search/index.md

Find a needle in a haystack in √N steps with amplitude amplification.
:::

:::{card} 🌊 12 · Quantum Fourier Transform & Phase Estimation
:link: lectures/12-qft-phase-estimation/index.md

The interference engine behind most famous quantum algorithms.
:::

:::{card} 🔓 13 · Shor's Algorithm
:link: lectures/13-shor-algorithm/index.md

Factoring integers with period finding, and what that means for RSA.
:::

::::

### 🔬 Phase 5 · Real Hardware & NISQ

Leave the ideal world: noise, error correction, hybrid algorithms and real QPUs.

::::{grid} 1 2 2 3
:class: roadmap-grid phase-5

:::{card} 🛡️ 14 · Noise, Decoherence & Error Correction
:link: lectures/14-noise-error-correction/index.md

Real qubits are fragile. Learn how errors happen and how to fight back.
:::

:::{card} 🎚️ 15 · Variational Algorithms (VQE & QAOA)
:link: lectures/15-variational-algorithms/index.md

Hybrid quantum–classical algorithms for today's noisy devices.
:::

:::{card} 🖥️ 16 · Running on Real Quantum Hardware
:link: lectures/16-real-hardware/index.md

Transpile, submit and interpret jobs on a real quantum processor.
:::

::::

### 🚀 Phase 6 · Projects

Put everything together and run a real quantum experiment.

::::{grid} 1 2 2 2
:class: roadmap-grid phase-6

:::{card} 🎯 17 · Project 1
:link: lectures/17-project-1/index.md

Build and analyse a quantum protocol end to end.
:::

:::{card} 🏆 18 · Project 2
:link: lectures/18-project-2/index.md

The capstone: design, run and report on a quantum experiment.
:::

::::

## 🧑‍🔬 How to use this course

::::{grid} 1 1 3 3

:::{card} 📑 Read the slides
Each lecture page hosts the slides for that session. Skim them before class and come back to them after.
:::

:::{card} 📓 Simulate everything
Run every notebook and change the circuits. A qubit you have simulated yourself is much easier to understand.
:::

:::{card} 🖥️ Then go real
Once a circuit works in simulation, run it on a real quantum processor and see what noise does to it.
:::

::::
