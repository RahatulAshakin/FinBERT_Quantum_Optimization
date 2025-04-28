# FinBERT Quantum Optimization Project

## Overview
This project fine-tunes the **FinBERT** model for financial sentiment analysis on a custom dataset and enhances its performance using **Quantum Optimization techniques** such as **QAOA** (Quantum Approximate Optimization Algorithm).

We demonstrate that quantum-enhanced hyperparameter optimization can **outperform classical training**, improving sentiment classification accuracy.

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
