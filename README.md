Micrograd & Neural Network Fundamentals
A lightweight Educational Repository based on Andrej Karpathy's lectures on Building Micrograd and Understanding Backpropagation from Scratch.

This project implements a custom Automatic Differentiation Engine (Autograd) and explores key concepts of Machine Learning, Data Structures, and Computational Graphs.

📌 Core Concepts Covered
- Value Class: A custom wrapper object tracking data, gradients, operational history, and parent nodes.
- Forward Pass: Step-by-step computation of expressions through mathematical operations (+, *, tanh, exp).
- Backward Pass (Backpropagation): Automatic computation of partial derivatives across computational graphs using Topological Sort.
- The Chain Rule: Application of $\frac{\partial L}{\partial x} = \frac{\partial L}{\partial y} \cdot \frac{\partial y}{\partial x}$ to propagate gradients from output loss to input weights.
- Graph Visualization: Rendering computational graphs with Graphviz to inspect node data and gradients.

Structure
├── micrograd/
│   ├── engine.py      # Core Value class & Autograd mechanics
│   └── nn.py          # Neuron, Layer, and MLP implementations
├── notebooks/
│   └── micrograd_walkthrough.ipynb  # Step-by-step lecture walkthrough
├── requirements.txt   # Dependencies (graphviz, etc.)
└── README.md
