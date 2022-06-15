# Camputer-Quantum-Programming

``Quantum Programming : Languages, SDKs &amp; Algorithms``

Quantum computers are expected to reduce power consumption from 100 to 1000 times because they operate at very low temperature at which the processor would work as a superconductor (i.e. it can conduct electricity with virtually no resistance).

On the other hand, quantum computers could accelerate machine learning processes, reducing thousands of years of learning to mere seconds. 

Quantum computers are based on quantum bits (Qubits) which have two possible values 0 or 1. 

They do not obey Newtonian laws but quantum laws allowing them to have the probability of being 0 and 1 at the same time. 

``Confused yet? ``

Then head to our article which explains what quantum computing is and how it works.

Due to the potential of quantum computers (QC), tech giants like Google and IBM are giving the opportunity to users who do not have QCs to learn how to program and manipulate quantum circuits using different quantum programming languages:

```Quantum programming languages```

Quantum programming languages are the foundations to interpret ideas into instructions to be carried out by a quantum computer. 

According to Nature Reviews, quantum programming languages are used to:

manage existing physical devices
predict quantum algorithms’ execution costs on possible devices
examine quantum computing concepts (qubits, superposition, entanglement)
test and verify quantum algorithms and their implementations
Current quantum programming languages and compilers are mainly focused on optimizing low-level circuits consisting of quantum gates. Quantum gates are the building blocks of quantum circuits. 

They are similar to reversible logic gates such as Fredkin gate, Toffoli gate, interaction gate, and switch gate. However, the smallest classical reversible gate has to use three bits, whereas the smallest quantum gate needs to use only two bits.

![quantum-gates-560x688 png (1)](https://user-images.githubusercontent.com/13979489/173781370-913b9704-11ba-494b-a0f3-9a7f9c34adee.png)



## Most quantum programming is done in 3 types of languages:

Imperative quantum programming languages



![imperative-quantum-language-560x349 jpg](https://user-images.githubusercontent.com/13979489/173781611-bdb5b0f4-80bd-4a67-b941-12bc31af55db.png)



Imperative programming languages consist of step-by-step instructions to be performed in order to accomplish the desired result. 

``In classical computers imperative languages include C, JavaScript, Pascal, Python, etc. The most popular quantum imperative languages are:``

QCL: Quantum Computing Language, one of the first implemented quantum programming languages. 

It resembles C language in regards of syntax and data types.
QMASM: Quantum Macro Assembler, published in 2016. It is a low-level language specific to quantum annealing. 

The significance of QMASM is that it relieves the programmer from having to know system-specific hardware details while still allowing programs to be expressed at a low level of abstraction.


Silq is originally published in 2020. Silq is a high-level programming language written in D language which has 482 stars and 10 contributors on github and is regularly updated as of 2021.


Other imperative Q languages include Quantum pseudocode, Q|SI>, Q language, qGCL, and Scaffold.

![functional-quantum-language jpg](https://user-images.githubusercontent.com/13979489/173781791-2b451bfe-944c-4d9c-a0ef-6a27fe9d2208.png)








## QCL - PROGRAMMING LANGUAGE


Quantum Programming Language
Quantum Programming Language is a programming language, which can be used to write programmes for quantum computer.

Since every quantum machine has to be controlled by classical device, existing quantum programming languages incorporate classical control structures such as loops and conditional execution and allow to operate on classical and quantum data.

Imperative quantum programming
Quantum pseudocode
Quantum pseudocode proposed by E. Knill is the first formalised language for description of quantum algorithms was introduced and, moreover, it was tightly connected with model of quantum machine called Quantum Random Access Machine (QRAM).


Quantum Computing Language
QCL (Quantum Computer Language) is the most advanced implemented quantum programming language. Its syntax resambles syntax of the C programming language and classical data types are similar to data types in C.

The basic built-in quantum data type in QCL is qreg (quantum register). It can be interpreted as a an array of qubits (quantum bits).

qureg x1[2]; // 2-qubit quantum register x1 qureg x2[2]; // 2-qubit quantum register x2 H(x1); // Hadamard operation on x1 H(x2[1]); // Hadamard operation on the first qubit of the register x1

Since qcl interpreter uses qlib simulation library, it is possible to observe internal state of the quantum machine during execution of the quantum programme.

qcl&gt; dump : STATE: 4 / 32 qubits allocated, 28 / 32 qubits free 0.35355 |0&gt; + 0.35355 |1&gt; + 0.35355 |2&gt; + 0.35355 |3&gt; + 0.35355 |8&gt; + 0.35355 |9&gt; + 0.35355 |10&gt; + 0.35355 |11&gt;

Note that dump operation is diffrent from measurement, since it does not influence the state of the quantum machine and can be realised only using simulator.

QCL standard library provides standard quantum operators used in quantum algorithms such as:

controlled-not with many target qubits,

Hadamard operation on many qubits,

parse and controlled phase.
