# ML-Learn — Machine Learning 

A practical, self-paced course covering machine learning from **scikit-learn fundamentals** to **gradient boosting** and **deep learning with PyTorch**.

Three Jupyter notebooks combine explanations, runnable examples, and hands-on exercises. The focus is on understanding models, evaluating them correctly, and building practical skills.

> The course notebooks are written in Ukrainian.

## Who This Course Is For

This course is for learners who know basic Python and want a structured introduction to machine learning.

Recommended background:
- Python functions, loops, and basic classes;
- basic NumPy and pandas operations;
- introductory statistics: means, variance, and probability.

No previous experience with neural networks is required.

## Course Contents

| Part | Topics | Notebook |
|---|---|---|
| **1. ML Fundamentals** | Feature types, train/test splits, regression, classification, metrics, cross-validation, pipelines, regularization, trees, clustering, and an introduction to deep learning | [Open notebook](./ml_course_sklearn_to_dl.ipynb) |
| **2. Tabular ML and Boosting** | Feature engineering, XGBoost, LightGBM, CatBoost, early stopping, interpretation, calibration, ensembles, and time-based validation | [Open notebook](./ml_part2_boosting_pro.ipynb) |
| **3. PyTorch and Deep Learning** | Tensors, autograd, training loops, MLPs, regularization, optimizers, CNNs, saving models, and GPU usage | [Open notebook](./ml_part3_pytorch_dl.ipynb) |

Each part includes practical exercises. Empty code cells following the exercises are provided for your solutions.

## How to Study

1. Work through the notebooks in order: **1 → 2 → 3**.
2. Run the cells from top to bottom and inspect the results.
3. Change parameters and observe how model behavior changes.
4. Complete the exercises independently and record your conclusions.
5. Apply what you learn in a separate project using an open dataset.

Pay particular attention to **validation, metric selection, and preventing data leakage**. These determine whether your model evaluation is reliable.

## Running Locally

You will need a Python 3 version supported by the libraries below.

Clone the repository:

```bash
git clone https://github.com/EternalSecond/ML-Learn.git
cd ML-Learn
```

Create a virtual environment:

```bash
python -m venv .venv
```

Activate it.

**Windows PowerShell:**

```powershell
.\.venv\Scripts\Activate.ps1
```

**Linux / macOS:**

```bash
source .venv/bin/activate
```

Install the dependencies:

```bash
python -m pip install --upgrade pip
python -m pip install jupyterlab numpy pandas matplotlib scipy scikit-learn
python -m pip install xgboost lightgbm catboost
python -m pip install torch torchvision
```

For the optional SHAP examples in Part 2:

```bash
python -m pip install shap
```

Start JupyterLab:

```bash
jupyter lab
```

Open a notebook and select the Python kernel with the installed dependencies.

> A CPU is sufficient for the course examples. For NVIDIA GPU support, use the installation command recommended for your system on the [PyTorch website](https://pytorch.org/get-started/locally/).

## Viewing and Running in a Browser

You can view the notebooks directly on GitHub without installing Python.

To run them in [Google Colab](https://colab.research.google.com/), open the **GitHub** tab in Colab or upload a notebook manually. Install any additional dependencies in the Colab environment as needed.

## Practice Projects

Suggested project directions include:
- classification and regression on open tabular datasets;
- customer churn prediction;
- demand forecasting with time-based validation;
- integrating an ML model into a web application;
- image classification and further exploration of transfer learning.

For each completed project, document the problem, data, validation strategy, metrics, results, and model limitations.

## Authorship and AI Assistance

This course was created by **EternalSecond**, with assistance from **Claude (Anthropic)** in preparing some of the materials.

This is an independent educational project. It is not an official course from Anthropic or the developers of the libraries used.

## Feedback and Contributions

Found an error, an unclear explanation, or a technical issue? Open an **Issue** and include the notebook name and relevant section.

Corrections and improvements to explanations, exercises, and code examples are welcome through **Pull Requests**.

## Licensing and Attribution

Textual explanations and educational content are licensed under
[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

When sharing the original materials or an adaptation, you must credit
**EternalSecond**, link to the source and license, and indicate any changes.
You may not present the original course materials as your own work.

Code in the notebooks is licensed under **Apache License 2.0**.
See [LICENSE](./LICENSE) for the full terms.

Third-party libraries, datasets, and external materials remain subject to their own licenses and terms.
