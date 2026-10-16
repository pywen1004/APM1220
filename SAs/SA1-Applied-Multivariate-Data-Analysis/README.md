# Multivariate Analysis of the Physicochemical Characteristics of Portuguese Vinho Verde Wines

## Study Title
**Multivariate Analysis of the Physicochemical Characteristics of Portuguese Vinho Verde Wines**

## Research Questions
This project investigates the physicochemical characteristics of wine to answer three major questions:
1. **MANOVA:** Do red and white wines differ significantly in their overall physicochemical characteristics when several characteristics are considered simultaneously[cite: 3]?
2. **PCA:** Can the 11 physicochemical measurements of wine be summarized using a smaller number of principal components while retaining a substantial proportion of the total variability[cite: 3]?
3. **EFA:** What underlying latent dimensions or factors explain the relationships among the physicochemical characteristics of wine[cite: 4]?

## Dataset Description
The dataset contains physicochemical measurements of Portuguese Vinho Verde wines[cite: 2]. It is a combined dataset of 6,497 total observations, comprising 1,599 red wine samples and 4,898 white wine samples[cite: 2]. The dataset contains 11 continuous physicochemical variables (such as fixed acidity, volatile acidity, residual sugar, chlorides, sulfur dioxide, density, pH, sulphates, and alcohol), a sensory quality score, and a categorical variable (`color`) identifying the wine as red or white[cite: 2, 3].

## Dataset Source & Attribution
*   **Source:** UCI Machine Learning Repository - Wine Quality Dataset (https://archive.ics.uci.edu/dataset/186/wine+quality)[cite: 2].
*   **Original Creators:** Cortez, P., Cerdeira, A., Almeida, F., Matos, T., & Reis, J. (2009). *Modeling wine preferences by data mining from physicochemical properties*. Decision Support Systems, 47(4), 547-553[cite: 15].
*   **License:** This dataset is licensed under a Creative Commons Attribution 4.0 International (CC BY 4.0) license[cite: 15].

## Statistical Methods
The following multivariate statistical techniques were applied to the dataset[cite: 2]:
*   **Data Preparation & Exploratory Data Analysis (EDA):** Dataset merging, outlier detection via Mahalanobis distance, and correlation analysis[cite: 4, 5].
*   **Multivariate Analysis of Variance (MANOVA):** Used to test for significant differences between red and white wines across multiple chemical variables simultaneously[cite: 2, 5].
*   **Principal Component Analysis (PCA):** Applied to standardized data to reduce the dimensionality of the 11 chemical features into a smaller set of principal components[cite: 2, 6, 7].
*   **Exploratory Factor Analysis (EFA):** Utilized to identify underlying latent constructs driving the chemical makeup of the wines[cite: 2, 8].

## Summary of Major Findings
*   **MANOVA:** Red and white wines exhibit profound, statistically significant differences across their combined chemical properties ($p < 0.001$)[cite: 28]. Red wines display higher volatile acidity and chlorides, while white wines are heavily defined by elevated total and free sulfur dioxide levels[cite: 28].
*   **PCA:** The 11 physicochemical variables were successfully reduced to 4 principal components, which together account for 73.19% of the total cumulative variance in the dataset[cite: 31, 36]. These components capture dimensions related to physical body/alcohol, sulfur dioxide preservation, acid/tartness balance, and volatile impurities[cite: 35, 36].
*   **EFA:** While the data exhibited a low Kaiser-Meyer-Olkin (KMO) sampling adequacy score (0.4053), the analysis mapped the shared variance of the chemical measurements to interpretable latent enological practices, separating variables into constructs like preservation management, natural grape acidity, and fermentation profiles[cite: 36].

## Software Used
*   **Language:** Python 3[cite: 18]
*   **Environment:** Jupyter Notebook / Google Colab[cite: 14, 19]
*   **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`, `statsmodels`, `scikit-learn`, and `factor_analyzer`[cite: 14, 19, 25, 26, 28, 30, 36].

## Instructions for Reproducing the Analysis
To reproduce the findings of this study, follow these steps:
1. Clone this repository to your local machine.
2. Ensure that Python 3 and the required libraries (`pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`, `statsmodels`, `scikit-learn`, `factor-analyzer`, `pingouin`) are installed.
3. Verify that the dataset files (`winequality-red.csv` and `winequality-white.csv`) are located in the `data/` directory[cite: 13].
4. Open the Jupyter Notebook file (`code/APM1220_SA1_SANTIAGO_TUPAS.ipynb`).
5. Run the cells sequentially to perform data preparation, EDA, MANOVA, PCA, and EFA. Ensure the dataset paths in the initial data import block correctly point to your local `data/` folder[cite: 19].
