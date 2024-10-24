markdown
# Customer Segments Analysis

This project focuses on identifying customer segments based on purchasing behavior data from a wholesale distributor. The analysis aims to uncover meaningful insights into different types of clients, such as supermarkets, cafes, and restaurants, using clustering techniques. The results help in understanding patterns within the data that can inform business strategies for targeted marketing and inventory management.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Analysis Steps](#analysis-steps)
- [Clustering Techniques Used](#clustering-techniques-used)
- [Results](#results)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)

## Project Overview
The main objective is to segment customers into different groups based on their purchasing patterns. Unsupervised learning techniques, specifically clustering algorithms, are used to identify distinct segments in the dataset. The analysis provides insights into customer types and their spending habits, potentially guiding business strategies in customer engagement, inventory management, and marketing.

## Dataset
The dataset used in this project contains annual spending data on various product categories for 440 clients of a wholesale distributor. The features in the dataset include:
- Fresh
- Milk
- Grocery
- Frozen
- Detergents_Paper
- Delicatessen

## Project Structure
- `customer_segments.ipynb`: The Jupyter notebook containing the full analysis, including data preprocessing, exploratory data analysis (EDA), and clustering.
- `README.md`: This file, which provides an overview of the project.

## Analysis Steps
1. **Data Exploration**: Initial exploration of the dataset, including summary statistics and distribution plots to understand the data.
2. **Data Preprocessing**:
   - Log-transforming the data to reduce skewness.
   - Scaling the data to normalize the features.
   - Detecting and removing outliers using Principal Component Analysis (PCA).
3. **Exploratory Data Analysis (EDA)**:
   - Visualization of the distribution of features.
   - Interpretation of statistical characteristics.
4. **Dimensionality Reduction**:
   - PCA is applied to reduce the number of features while retaining variance.
   - Two principal components are selected for visualization.
5. **Clustering**:
   - Clustering algorithms like K-Means and Gaussian Mixture Models (GMM) are used to identify potential segments.
   - Cluster centers are analyzed to characterize each segment.

## Clustering Techniques Used
The analysis employed the following clustering algorithms:
- **K-Means Clustering**: This algorithm partitions the dataset into a specified number of clusters, where each data point belongs to the cluster with the nearest mean.
- **Gaussian Mixture Model (GMM)**: This probabilistic model assumes that the data points are generated from a mixture of several Gaussian distributions.

## Results
The clustering analysis identified the following customer segments:
- **Segment 0**: Represents supermarkets. Customers in this segment tend to spend higher than the median on Milk, Grocery, Detergents_Paper, and Deli products.
- **Segment 1**: Represents restaurants. Customers in this segment spend more on Fresh and Frozen items, but less on Milk, Grocery, and Detergents_Paper.

Sample points were used to validate the clustering results, with mixed accuracy in identifying segment membership based on original assumptions.

## Installation
To run this project, ensure you have Python installed along with the necessary libraries:
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

You can install these dependencies using:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

## Usage
1. Clone this repository:
   ```bash
   git clone https://github.com/your_username/customer_segments.git
   ```
2. Navigate to the project directory:
   ```bash
   cd customer_segments
   ```
3. Open the Jupyter notebook:
   ```bash
   jupyter notebook customer_segments.ipynb
   ```

4. Run the cells in the notebook to execute the analysis.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any suggestions or improvements.
