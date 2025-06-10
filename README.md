# Modeling Human-Like Learning in AI: Evaluating RNNS Capacity to Replicate Human Leaps of Insight in Sequential Decision making

This repository contains the code and research artifacts from my senior thesis in Computational Neuroscience at the Claremont Colleges. The project investigates whether Recurrent Neural Networks (RNNs), particularly LSTMs, can replicate human "leaps of insight"—sudden strategic breakthroughs—in sequential decision-making tasks.

---

## 🎯 Project Overview

Humans often solve complex problems not just through trial-and-error, but through sudden shifts in understanding. This research explores how AI, which typically learns iteratively and incrementally, compares to human learning in this regard.

Using gameplay data from **Hexxed.io**, a six-lobed puzzle game where players learn through exploration without instructions, I trained and evaluated various neural models to:

- Predict human actions based on previous moves and board states  
- Compare the effectiveness of different architectures (dense vs. RNNs)  
- Assess whether AI can simulate cognitive leaps via bottom-up learning  

---

## 🧠 Core Research Questions

- Can RNNs emulate top-down cognitive shifts using bottom-up learning mechanisms?  
- Do temporal dependencies improve predictive accuracy in human-like learning scenarios?  
- Which input features (board state vs. previous action) contribute more to model performance?

---

## 📁 Repository Contents

- `Github_copy_of_Winners_Only.ipynb`: Main notebook for training, testing, and analyzing RNN models on Hexxed gameplay data.  
- `data/`: (If available) Processed and padded gameplay sequences from Hexxed.io.  
- `models/`: Control models, RNN architectures, and masked loss functions.  
- `figures/`: Visuals including accuracy curves, confusion matrices, and architecture diagrams.  
- `thesis/`: [Optional] Full thesis PDF or DOCX if included for context.

---

## 📈 Key Results

- A single-layer LSTM model outperformed dense control networks, achieving ~68% validation accuracy.  
- Temporal structure was more important than depth or non-linearity for modeling behavior.  
- RNNs captured aspects of strategic learning but failed to replicate true "leaps of insight."

---

## 🧰 Tools & Frameworks

- Python  
- TensorFlow / Keras  
- Optuna (for hyperparameter tuning)  
- NumPy, Pandas, Matplotlib

---

## 🧪 Future Directions

- Incorporate reinforcement learning to simulate top-down learning signals like reward and motivation.  
- Expand dataset to longer and more diverse player sequences.  
- Integrate reward feedback (e.g., score) into the modeling pipeline.

---

## 📜 Citation

If referencing this work, please cite:

> Mizrahi, N. L. (2024). *Modeling Human-Like Learning in AI: Evaluating Recurrent Neural Networks' Capacity to Replicate Human Leaps of Insight in Sequential Decision-Making.* Senior Thesis, Claremont McKenna, Scripps, and Pitzer Colleges.
