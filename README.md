

# Facebook Friend Recommendation System

This project focuses on predicting missing links in a directed social graph, specifically for recommending friends on Facebook. It applies various machine learning and graph-based algorithms to make accurate friend recommendations.

## Dataset
- **Source**: Facebook Recruiting Challenge on Kaggle.
- **Features**: `source_node`, `destination_node` (representing users in a directed graph).
  
## Problem Statement
- **Objective**: Predict missing links in a directed social graph (recommend friends based on the graph structure).

## Techniques Used
1. **Feature Engineering**:
   - Generated features like **number of followers**, **PageRank**, **Katz Centrality**, **Adamic/Adar Index**, and **Jaccard Similarity** for both source and destination nodes.
   - Calculated the shortest path and whether nodes belong to the same weakly connected component.

2. **Graph Algorithms**:
   - Used **PageRank**, **Hits Algorithm**, and **Katz Centrality** to compute node importance and influence in the graph.
   - Applied **Cosine Similarity** and **Jaccard Index** to measure similarity between users based on their followers and followees.

3. **Machine Learning**:
   - Trained models like **Random Forest** and **XGBoost** using the extracted features.
   - Evaluated the model's performance using F1 score and Confusion Matrix.

## Results
- **Best Model Performance**: Achieved strong prediction accuracy using Random Forest and XGBoost classifiers.
- **Evaluation Metrics**: High precision and recall in predicting friend recommendations.

## Conclusion
This project effectively predicts friend recommendations by leveraging graph-based features and machine learning algorithms, helping improve the social network experience.

