# Modeling Human-Like Learning in AI: Evaluating RNNs' Capacity to Replicate Human Leaps of Insight in Sequential Decision-Making

This repository contains the code and research artifacts from my senior thesis in Computational Neuroscience at the Claremont Colleges. The project investigates the extent that Recurrent Neural Networks (RNNs), particularly LSTMs, can replicate human "leaps of insight"—sudden strategic breakthroughs—in sequential decision-making tasks.

**Note:** Certain gameplay outputs and original user data from Hexxed.io were redacted to protect participant confidentiality.

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

- `Player_Gameplay_Data_Preprocessing.ipynb`: Processes raw user action sequences and generates board state/action datasets.
- `Control_Models.ipynb`: Implements and evaluates linear and nonlinear dense control models.
- `RNNs.ipynb`: Builds 3 RNN architectures with varying LSTM layers to model sequential dependencies. Includes custom masked loss and accuracy functions
- `Model_Comparison.ipynb`: Compares performance of RNNs vs control models, including feature ablations.
- `Sequence_Tracking.ipynb`: Analyzes accuracy across sequence steps to evaluate temporal modeling.
- `NMizrahiPoster.pdf`: A one-page visual summary of the experiment, methods, and key findings.
- `thesis/`: Full thesis PDF for academic context.

> 📌 All notebooks were originally developed in a single file and later split into modular parts for ease of navigation. For best results, follow the order listed above.

> 🔁 All notebooks were re-run for GitHub upload and may show minor differences in results compared to the thesis and poster due to retraining variance.

---

## 📈 Key Results

- A single-layer LSTM model outperformed dense control networks, achieving ~69% validation accuracy.  
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

> Mizrahi, N. L. (2024). *Modeling Human-Like Learning in AI: Evaluating Recurrent Neural Networks' Capacity to Replicate Human Leaps of Insight in Sequential Decision-Making.* Senior Thesis, Scripps College, W. M. Keck Science Department.
