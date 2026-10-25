# Artificial Intelligence Fundamentals & Applications - Lab 1 Assignment

## Project Overview
The overall assignment integrates core AI concepts, specifically **Classical Search Algorithms** (BFS, A* Search) and **Regularized Regression Modeling** (Linear vs. Ridge Regression). Designed with a low-code and conceptual problem-solving focus, this project demonstrates the application of Machine Learning using Scikit-Learn and interactive learning with Generative AI copilots.

## Repository Contents
* **`Horvath_Mate_Lab_Assignment_1.ipynb`**: The completed Google Colab notebook containing the Python code for:
  * Fetching and sampling the California Housing dataset.
  * Preprocessing and scaling continuous input features using `StandardScaler`.
  * Training and evaluating **Linear Regression** and **Ridge Regression** models.
  * Performing 5-Fold Cross-Validation for robust performance metrics ($R^2$ scores).
  * Visualizing the performance comparison across different L2 regularization penalties ($\alpha = 0.1, 10.0, 1000.0$).
* **`README.md`**: This detailed documentation file.

*The hand calculations for Part 1 - Graph Traversal and 8-Puzzle Problem using A* Search, along with the detailed AI Prompting Logs, are submitted as a separate PDF Report.*

## Machine Learning Experiment: Key Findings
In **Part 2: Applied Machine Learning**, we utilized the California Housing Dataset to predict continuous target variables (`MedHouseVal`). Key conceptual takeaways include:

1. **Feature Scaling:** Applying `StandardScaler` was crucial to ensure features with naturally large numerical ranges (like population) did not dominate the regression calculations over smaller-scaled features (like average rooms).
2. **Cross-Validation vs. Single Split:** Using 5-Fold Cross-Validation provided a much more reliable evaluation metric by testing the model across multiple slices of the data, reducing the risk of a "lucky" train/test split.
3. **Overfitting vs. Underfitting (Alpha Tuning):** 
   * A moderate Ridge penalty (e.g., $\alpha = 10.0$) helped generalize the model by preventing feature coefficients from becoming too large (overfitting). 
   * However, an extremely high penalty (e.g., $\alpha = 1000.0$) severely restricted the model's flexibility to learn patterns, causing performance to drop significantly due to underfitting.

## How to Run the Code
1. Download the `SC5002_ML_Assignment.ipynb` file from this repository.
2. Go to [Google Colab](https://colab.research.google.com/).
3. Click on **File > Upload notebook** and select the downloaded file.
4. Click on **Runtime > Run all** (or run the single cell directly) to execute the script and view the dataset rows, cross-validation scores, and the generated bar chart.

## AI Copilot Integration ("Learn with AI")
In accordance with the assignment guidelines, Generative AI (e.g., ChatGPT / Gemini / Claude) was actively used as an interactive learning partner throughout this project. It assisted in:
* Clarifying theoretical concepts such as "admissible heuristics" using real-world GPS analogies.
* Verifying node-selection decisions in the A* Search 8-Puzzle problem.
* Synthesizing the impact of L2 Regularization and the bias-variance tradeoff in layman's terms for non-technical audiences.

---
**Author:** [Your Name]  
**Course:** SC5002 - Artificial Intelligence Fundamentals & Applications  
**Institution:** Nanyang Technological University (NTU)
