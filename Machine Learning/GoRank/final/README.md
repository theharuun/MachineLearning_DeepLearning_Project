# Sparsity-Aware Hybrid Recommendation System

## Project Overview
This project presents a novel, sparsity-aware hybrid recommendation pipeline. It dynamically integrates Collaborative Filtering (optimized SVD) with Content-Based structural similarities (Gower's Coefficient - GoRank) using a deterministic, data-driven "User Density Ratio." This repository/archive contains the final source code and all supporting academic documentation submitted for the Final Project.

## Archive Contents
The submitted `.zip` / `.rar` archive contains the following files:

1. **`final.ipynb`**: The main Jupyter Notebook containing the complete, executable Python code. It includes data preparation, hyperparameter optimization (GridSearchCV), K-Fold cross-validation, the sparsity-aware hybridization logic, and final NDCG evaluations.
2. **`report1_article.docx`**: The primary academic paper detailing the theoretical background, proposed approach, experimental setup, and performance analysis formatted according to international academic standards.
3. **`report2_difference.docx`**: A one-page summary highlighting the substantial methodological improvements made between the midterm and the final project.
4. **`report3_code_review.docx`**: A comprehensive, line-by-line technical documentation and explanation of the Jupyter Notebook cells.
5. **`README.md`**: This instruction file.

## Prerequisites & Installation
To execute the code successfully, you need Python 3.x installed on your system along with Jupyter environment. The code relies on standard data science libraries and the `scikit-surprise` library for matrix factorization.

You can install all required dependencies using `pip` by running the following command in your terminal or command prompt:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn scikit-surprise

```

## Execution Instructions

1. Extract the contents of the submitted archive into a single local folder.
2. Open your terminal or command prompt and navigate to the extracted folder.
3. Launch Jupyter Notebook by typing:
```bash
jupyter notebook final.ipynb

```


*(Alternatively, you can open the `final.ipynb` file using Visual Studio Code or upload it to Google Colab).*
4. Once the notebook is open, select **"Run All"** from the Cell menu to execute the pipeline sequentially from top to bottom.
5. The dataset (MovieLens-100K) is fetched dynamically via a direct URL within the code, so no local dataset files are required. The script will automatically output all tables, prints, and comparative bar charts directly below the respective cells.

## Notes

* **Execution Time:** The GridSearchCV optimization phase (Cell 2) tests multiple parameters and performs cross-validation. Depending on your CPU, this cell may take 1-3 minutes to complete. Please allow the machine to finish processing.

