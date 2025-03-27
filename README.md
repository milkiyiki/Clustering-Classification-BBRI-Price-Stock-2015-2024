# Clustering and Classification of Bank BRI Stock Prices

## Project Description
This project aims to perform **clustering** on the Bank BRI stock price dataset from December 2015 to December 2024. After clustering, the results will be used as the basis for building a **classification model**. This analysis seeks to identify patterns in stock price movements and group data based on specific characteristics.

## Dataset
- **File Name**: `stock_price.csv`
- **Period**: December 2015 - December 2024
- **Number of Records**: > 2000 rows
- **Features Used**:
  - Open Price
  - Close Price
  - High
  - Low
  - Volume
  - Technical indicators (if available)

## Analysis Steps
### 1. **Data Exploration**
   - Checking data distribution
   - Cleaning data if necessary
   - Visualizing stock price trends

### 2. **Clustering**
   - **Method**: K-means clustering
   - **Evaluation**:
     - **Silhouette Score**: 0.7015 (indicating good clustering)
     - Cluster distribution:
       ```
       Cluster
       1    1725
       0     455
       ```
   - **Visualization**: PCA / t-SNE to observe cluster separation
   - **Alternative Algorithm**: DBSCAN for more flexible clustering possibilities

### 3. **Classification**
   - Using clustering results as labels to build a classification model
   - Models tested:
     - Logistic Regression
     - Decision Tree
     - Random Forest
     - SVM
   - **Evaluation**: Accuracy, Precision, Recall, F1-score

## Installation and Usage
1. Clone this repository:
   ```bash
   git clone https://github.com/username/repo.git
   cd repo
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run clustering analysis:
   ```python
   python clustering.py
   ```
4. Run classification model:
   ```python
   python classification.py
   ```

## Results and Conclusion
- Clustering shows a good separation of data with a Silhouette Score of 0.7015
- The classification model will be used to predict stock clusters based on price features
- Potential improvements: exploring additional features and tuning classification models

## Contributors
- **Risqie Nur Salsabila** (@milkiyiki)

## License
This project is licensed under the **MIT License**.

