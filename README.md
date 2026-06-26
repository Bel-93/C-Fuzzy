# C-Fuzzy

Comparing a popular, widely-used clustering algorithm (**K-Means**) against a clustering approach that is **arbitrarily robust to outliers** (**Fuzzy C-Means**), to highlight how each one behaves on the same data.

## 📌 About

This project explores the differences between **K-Means clustering** and **Fuzzy C-Means clustering**:

- **K-Means** is fast and simple, but sensitive to outliers and assigns each point to exactly one cluster.
- **Fuzzy C-Means** assigns each point a *degree of membership* to every cluster, making it more robust when the data contains noise or outliers.

The repository contains the notebook that walks through this comparison.

## 📂 Repository contents

| File | Description |
|---|---|
| `Conglomerados_Fuzzy.ipynb` | Main notebook: builds and compares K-Means vs. Fuzzy C-Means clustering. |
| `type` | Supporting file used by the notebook. |

## 🛠️ Requirements

- Python 3.9+
- Jupyter Notebook, JupyterLab, or Google Colab
- Libraries used in the notebook:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - `scikit-fuzzy` (installed via `pip install scikit-fuzzy`)
  - `scikit-learn` (for `StandardScaler`, and for K-Means if used in the comparison)

## 🚀 How to run it locally

### 1. Clone the repository

```bash
git clone https://github.com/Bel-93/C-Fuzzy.git
cd C-Fuzzy
```

### 2. Create a virtual environment (recommended)

```bash
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate
```

### 3. Install dependencies

If you add a `requirements.txt` file to the repo, just run:

```bash
pip install -r requirements.txt
```

Otherwise, install the libraries directly:

```bash
pip install pandas numpy matplotlib seaborn scikit-fuzzy scikit-learn jupyter
```

### 4. Launch Jupyter

```bash
jupyter notebook
```

This opens Jupyter in your browser. From there, open `Conglomerados_Fuzzy.ipynb` and run the cells in order (Cell → Run All, or step by step with `Shift + Enter`).

## ☁️ How to run it without installing anything (Google Colab)

1. Go to [Google Colab](https://colab.research.google.com/).
2. Click **File → Open notebook → GitHub**.
3. Paste the repository URL: `https://github.com/Bel-93/C-Fuzzy`
4. Open `Conglomerados_Fuzzy.ipynb`.
5. Run the first cell, which installs the only library Colab doesn't have by default:

```python
!pip install scikit-fuzzy
```

6. Run the rest of the cells normally.

## 📤 How to upload / push changes to GitHub

If you made local changes and want to push them back to your repository:

```bash
git add .
git commit -m "Update notebook"
git push origin main
```

If this is the **first time** pushing this project from a local folder (no `git clone` was done):

```bash
git init
git remote add origin https://github.com/Bel-93/C-Fuzzy.git
git add .
git commit -m "Initial commit"
git branch -M main
git push -u origin main
```

## 📄 License

No license specified yet. Consider adding one (e.g. MIT) if you want others to reuse this code.
