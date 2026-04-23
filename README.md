# 1993639_Fondamenti_di_IA
## Homework Summary: Fondamenti di IA (A.A. 2023/24)

This project focuses on the analysis and application of various Machine Learning algorithms to a dataset designed for estimating **obesity levels** in individuals from Mexico, Peru, and Colombia, based on their dietary habits and physical attributes.

### 1. Data Preprocessing and Cleaning
* **Feature Engineering**: Categorical and alphabetical data (such as meal frequency or lifestyle habits) were mapped to numerical values. This involved converting binary variables into 0/1 and frequency-based descriptors into percentages/scales.
* **Task-Specific Adaptation**: The dataset was prepared in two distinct formats: one optimized for **regression** tasks and another for **classification** tasks.

### 2. Implementation of Models "From Scratch"
The core of the homework involved the manual implementation (without high-level libraries for the core logic) of the following algorithms:
* **Linear Regression**: Implemented using both the **Moore-Penrose pseudo-inverse** (analytical solution) and the **Stochastic Gradient Descent (SGD)** optimization algorithm.
* **Decision Trees**: Developed for predictive logic based on attribute splitting.
* **Logistic Regression**: Implemented for classification purposes.
* **K-Nearest Neighbors (KNN)**: A distance-based algorithm implemented to classify instances based on feature space proximity.
* **Neural Networks**: A custom implementation including the design of the architecture and the **backpropagation** algorithm for weight updates.

### 3. Hyperparameter Tuning and Benchmarking
* **Optimization**: Extensive tuning was performed for each model to identify the best parameters, such as learning rates, batch sizes, and the number of hidden layers/nodes in the neural network.
* **Validation**: The performance of the custom-built models was directly compared against standard industry benchmarks (e.g., `scikit-learn`) using metrics such as **MSE (Mean Squared Error)** and **RMSE**, supported by data visualization.

### 4. Final Comparative Analysis
The work concludes with a technical evaluation of the performance, strengths, and weaknesses of each approach:
* **Decision Trees**: High precision but significant memory footprint for large datasets.
* **KNN**: Accurate but suffers from high computational latency during the prediction phase since no prior training is performed.
* **SGD & Logistic Regression**: Fast and scalable, though sensitive to feature scaling and high-dimensional data.
* **Neural Networks**: Highly versatile and capable of modeling complex patterns, though sensitive to architectural configuration.
