# BDH-MEMORY-VISUALIZATION
Visualization of memory dynamics and sparsity inspired by Dragon Hatchling (BDH)
Track 2 – The Frontier | Path B: Visualization & Inner Worlds

Overview
This project explores how memory forms and evolves in a brain-inspired, post-transformer setting, motivated by the Dragon Hatchling (BDH) architecture.
Instead of focusing on task accuracy, the goal is to make memory dynamics visible at the neuron and synapse level.
Transformers rely on dense matrix operations that make memory opaque and difficult to interpret.
BDH, on the other hand, introduces sparsity and biological learning rules, enabling memory to be represented as an evolving graph.
This project visualizes those ideas.

Track Alignment
Hackathon: Synaptix Frontier AI Hack @ IIT Madras (Shaastra 2026)
Track: Track 2 – The Frontier
Path: Path B – Visualization and Inner Worlds
This is a BDH-inspired experimental study focused on visualization and interpretability.
It does not attempt to re-train or fully reproduce the official BDH model.

What This Project Demonstrates
Sparse neural activation over time (~5%)
Hebbian learning: synapses strengthen through repeated co-activation
Emergent graph-based memory topology
Neuron-level synaptic inspection
Real-time memory formation dynamics

Methodology
Neurons are modeled as nodes in a graph, and memory is represented as weighted synaptic connections.
When a group of neurons activates together, the synapses between them strengthen following a Hebbian update rule:
“Neurons that fire together wire together.”

Two data sources are used:
Synthetic patterns for controlled, noise-free experiments
MovieLens 100K dataset to validate the same behavior on real-world interaction data

Key Observations
Dense activation leads to rapid growth but high overlap and noise
Sparse activation grows slower but forms cleaner and more interpretable structure
Early-stage sparse memory can appear nearly empty
Repeated exposure is required for stable structure to emerge
Neuron-level inspection reveals consistent synaptic patterns

Visual Results
The project includes multiple visualizations:
Activation density over time
Hebbian synapse strengthening animation
Emergent sparse graph topology
Neuron synaptic profiles
All generated images are available in the results/ folder.

Limitations
This work focuses on conceptual correctness and interpretability rather than performance benchmarking.
Linear attention, full BDH internals (Gx, σ matrices), and large-scale training are outside the scope of this study.

Why This Matters
Transformers struggle with long-term memory due to dense, overlapping representations.
This project shows how sparsity and biological learning rules naturally reduce interference and make memory interpretable — a core motivation behind BDH.

How to Run
Open bdh_memory_experiment.ipynb in Google Colab and run the cells from top to bottom.
