# FinBERT Quantum Optimization Project

## Overview
In current quantum computing experiments, pervasive noise and the lack of robust error
correction mechanisms pose significant challenges to reproducibility and result stability. Because
today’s quantum processors operate in the Noisy Intermediate-Scale Quantum (NISQ) regime
without full error correction, various error sources – including qubit decoherence, imperfect gate
operations (limited gate fidelity), inter-qubit crosstalk, and measurement (readout) errors – can
accumulate throughout a computation​. Qubit decoherence refers to the gradual loss of quantum
coherence as qubits interact with their environment, which causes quantum information to decay
into classical states​. This limits how long computations can run before the quantum state
essentially randomizes. Similarly, finite gate fidelities mean that each quantum logic gate has a
non-zero chance of introducing an error due to control pulse imperfections or calibration drift.
Crosstalk errors occur when operations on one qubit inadvertently disturb the state of a nearby
qubit due to unintended coupling or control signal leakage and have been identified as a
significant source of error in current hardware​. Meanwhile, readout errors during measurement
can cause the reported qubit state to be incorrect (e.g., reading a 0 as 1 or vice versa), further
skewing the results​. Collectively, these noise processes degrade the fidelity of quantum
operations and lead to high variability in outputs. Running the same algorithm multiple times can
yield fluctuating outcomes because random error fluctuations at each run accumulate differently,
undermining reliable reproducibility​. This noise-induced variability can also disrupt algorithmic
convergence – for instance, in iterative algorithms, noise can alter the measured objective
function and prevent consistent convergence to the same solution. Overall, current quantum
algorithm results often require statistical averaging over many runs to distinguish signal from
noise, and even then the results have significant uncertainty. While these limitations currently
constrain quantum computing experiments, ongoing advances in quantum error correction and
error mitigation techniques are expected to gradually improve fidelity and stability, bringing
more consistent and reproducible outcomes over time.
---

## Project Structure

| Folder/File | Purpose |
|:-----------|:--------|
| `/data/`    | Contains the dataset (`all-data.csv`) used for training. |
| `/models/`  | Saved models after fine-tuning and quantum optimization. |
| `/notebooks/` | Jupyter notebooks for model fine-tuning (`finetune.ipynb`) and quantum optimization (`QBert.ipynb`). |
| `/results/` | Output figures like loss curves, confusion matrices. |
| `.gitignore` | To ignore unnecessary files in version control. |
| `requirements.txt` | List of libraries needed to run the project. |
| `README.md` | Project documentation (this file). |

---

## Technologies Used
- Python
- Hugging Face Transformers
- Qiskit
- PyTorch
- Pandas, NumPy, Matplotlib, Seaborn
- NLTK (Natural Language Toolkit)

---

## How to Run

1. **Clone the repository**:
    ```bash
    git clone https://github.com/RahatulAshakin/FinBERT_Quantum_Optimization.git
    cd FinBERT_Quantum_Optimization
    ```

2. **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Open Notebooks**:
   - Open `notebooks/finetune.ipynb` to fine-tune FinBERT.
   - Open `notebooks/QBert.ipynb` to apply Quantum Optimization (QAOA, VQE).

4. **View Results**:
   - Confusion Matrix
   - Loss Curves
   - Classification Report

---

## Results

| Model | Accuracy |
|:------|:---------|
| Classical FinBERT | ~78% |
| FinBERT + QAOA Optimized | ~89% |

 Quantum optimization led to **~11% improvement** in classification accuracy compared to classical training.

## Download Pre-trained Model

We host the large `finbert_qaoa_optimized` model externally to keep this repo lightweight.

You can download the models from the below link:

"https://drive.google.com/drive/folders/1IWYWJ9Eu9UMh04-B2Dzeyf353pK42uBS?usp=sharing"

---

## Future Work
- Experiment with **Grover's Algorithm** for optimization.
- Scale up on **larger financial datasets**.
- Explore running QAOA/VQE on **real quantum hardware**.

---

## License
This project is licensed under the MIT License.  
Feel free to use, modify, and distribute it with attribution.

---

## Author
**[Md Rahatul Ashakin]**  
For any queries or collaboration, feel free to connect!
