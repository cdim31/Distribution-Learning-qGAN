# Quantum Generative Adversarial Networks for Distribution Learning
**Semester Project** - Introduction to Quantum Computing  
*Technical University of Crete, professor : Mr D. Angelakis*

## Repository Overview
This repository reproduces results from the paper:  
**"Quantum Generative Adversarial Networks for learning and loading random distributions"**  
(Christa Zoufal, Aurélien Lucchi, Stefan Woerner)

The Jupyter notebook implementation demonstrates:
- Quantum Generative Adversarial Network (qGAN) architecture
- Learning and loading random distributions using quantum circuits
- Comparative analysis with classical approaches

## Setup Instructions

### 1. Clone Repository
```bash
git clone https://github.com/your-username/Distribution-Learning-qGAN.git
cd Distribution-Learning-qGAN
```

### 2. Create and Activate Virtual Environment
```bash
python -m venv qgan-env
```

- **Linux/macOS**:
  ```bash
  source qgan-env/bin/activate
  ```
- **Windows**:
  ```cmd
  .\qgan-env\Scripts\activate
  ```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure Jupyter Kernel (Critical Step!)
```bash
python -m ipykernel install --user --name=qgan-env
```

## Running the Notebook
1. Start Jupyter from activated environment:
   ```bash
   jupyter notebook
   ```
2. In your browser:
   - Open `project_final.ipynb`
   - Verify kernel: **Kernel > Change Kernel > qgan-env**
3. Execute cells sequentially (Use **Kernel > Restart & Run All** for full execution)

## Expected Outputs
Successful execution will generate:
1. 20,000 samples of a lognormal distribution $x \in [0, 7]$.
2. Training loss curves for generator/discriminator
3. Quantum circuit diagrams for data loading
4. Comparative histograms (target vs. learned distributions)
5. Fidelity metrics at different training stages
6. Convergence plots showing training progress

## Project Notes
### Key Parameters (modify in notebook)
All the important key parameters are in the `Config` cell, in order to make it easier for everyone to experiment with different methods.

### Hardware Requirements
- **Simulation**: Nothing significant, really fast and effective.

### Reference Results
```
│ Metric          │ Value       │
├─────────────────┼─────────────┤
│ Relative Entropy|   0.0003    │
│ KS statistic    │   0.0081    │
│ Training Time   │   ~5 min    │
```

## References
1. Zoufal, C., Lucchi, A., & Woerner, S. (2019). [Quantum Generative Adversarial Networks for learning and loading random distributions](https://www.nature.com/articles/s41534-019-0223-2). *npj Quantum Information*
2. Qiskit Machine Learning Documentation: [qiskit.org/ecosystem/machine-learning](https://qiskit.org/ecosystem/machine-learning/)
