git add README.md
# CNN Basics with TensorFlow & Keras

A minimal, clean starter project to practice **Convolutional Neural Networks (CNNs)** using TensorFlow/Keras.
It includes a ready-to-run notebook (MNIST) and a small Python module that builds a simple CNN.

---

## 🗂 Project Structure

```
cnn-basics/
├─ notebooks/
│  └─ cnn_basics.ipynb       # Jupyter notebook: load data, build, train, evaluate, plot
├─ src/
│  └─ model.py               # Reusable CNN builder (Keras Sequential)
├─ data/                     # (optional) put your local datasets here (ignored by git)
├─ requirements.txt          # deps (TensorFlow 2.x, numpy, matplotlib)
├─ .gitignore                # ignore cache, venv, data
└─ README.md
```

---

## ⚙️ Setup

```bash
# (optional) create and activate a virtual environment
python -m venv .venv
source .venv/bin/activate

# install deps
pip install --upgrade pip
pip install -r requirements.txt
```

> **Note:** TensorFlow GPU requires additional drivers/CUDA. CPU-only is fine for this demo.

---

## 🚀 Quick Start

Run the Python module:
```bash
python src/model.py
```

Or open the notebook:
```bash
jupyter notebook notebooks/cnn_basics.ipynb
# or
jupyter lab notebooks/cnn_basics.ipynb
```

---

## 🧠 Model Outline (default)
```
Conv2D(32, 3x3, relu) → MaxPool(2x2)
Conv2D(64, 3x3, relu) → MaxPool(2x2)
Flatten → Dense(128, relu) → Dense(n_classes, softmax/sigmoid)
```

---

## 📌 Tips
- Start with MNIST (grayscale 28×28×1), then switch to your own images.
- Keep datasets out of git (use `data/` — already gitignored).
- Track improvements with clear commit messages (`feat:`, `fix:`, `docs:`).

---

## 👤 Author
**Milzon** — [milzon.ltf@gmail.com](mailto:milzon.ltf@gmail.com)
GitHub: https://github.com/milzon1010
