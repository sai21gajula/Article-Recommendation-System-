
# Cluster Based Article Recommender System

## Project Overview
This project develops an advanced article recommendation system that leverages machine learning and natural language processing (NLP) techniques to provide personalized article recommendations. The system combines content-based filtering, principal component analysis (PCA) for dimensionality reduction, and TF-IDF vectorization to create a sophisticated tool for recommending articles based on user preferences and content relevance.

## Key Features
- **Content-Based Filtering**: Analyzes the content of articles and matches them with user profiles created from their past interactions, ensuring recommendations are personalized and relevant.
- **Principal Component Analysis (PCA)**: Employs PCA to reduce the dimensionality of the TF-IDF features, which improves the efficiency of the recommendation engine and focuses on the most significant features.
- **TF-IDF Vectorization**: Converts text data into a feature matrix where each word or phrase's importance is inversely proportional to its frequency across all documents, highlighting unique aspects of each article.

## System Requirements
- Python 3.8+
- Libraries: NumPy, pandas, matplotlib, SciPy, sklearn, nltk, spacy

## Installation
```bash
# Clone this repository
git clone https://github.com/your-username/advanced-article-recommender.git

# Navigate to the project directory
cd advanced-article-recommender

# Install required Python packages
pip install -r requirements.txt
```

## Usage
Download the notebook and run the notebook in the google colab or jupyter notebook.

## Data Description
- **Articles Dataset**: Contains detailed metadata for each article including title, author, and the full text content.
- **User Interactions Dataset**: Includes data on user actions (e.g., views, likes, and shares) which is used to construct dynamic user profiles.

## Data Preprocessing
- **Text Normalization**: Includes converting text to lowercase, removing punctuation and special characters, and stripping extra spaces.
- **Stop Words Removal**: Filters out common words that do not contribute to the semantic meaning of the texts.
- **Tokenization**: Splits text into individual elements or tokens.
- **TF-IDF Application**: Transforms the cleaned text into a numerical representation that highlights the most important words.

## Visualization
- **PCA Variance Plot**: Displays a line plot of the cumulative variance explained by the principal components to determine how many components are necessary for a good balance of information retention and feature reduction.
- **Recommendation Strength Distribution**: Visualizes the strength of recommendations using histograms or bar charts to evaluate the model's confidence in its suggestions.

## Evaluation Metrics
- **Hit Rate**: Measures whether the recommended articles are relevant to the user's interests.
- **Precision and Recall**: Assesses the accuracy of the recommendations in terms of relevance and completeness.
- **F1 Score**: Combines precision and recall into a single metric to provide a balanced view of model performance.
- **NDCG (Normalized Discounted Cumulative Gain)**: Evaluates the ranking quality of the recommended articles, giving more importance to highly relevant articles appearing earlier in the list.

### Model Performance

#### Hybrid Model:
- **Recall@5**: 0.316287
- **Recall@10**: 0.434416
- **MRR**: 0.445120
- **NDCG**: 0.526664

#### Collaborative Filtering:
- **Recall@5**: 0.268346
- **Recall@10**: 0.401048
- **MRR**: 0.264244
- **NDCG**: 0.548831

#### Content-Based:
- **Recall@5**: 0.188187
- **Recall@10**: 0.271925
- **MRR**: 0.294764
- **NDCG**: 0.495701

### Key Insights

- The hybrid recommendation model demonstrates superior performance in terms of recall and MRR, making it the best overall model for recommending relevant items.
- The collaborative filtering model excels in ranking quality, as indicated by the highest NDCG, though it falls behind in recall metrics.
- The content-based model performs the least effectively among the three.

---

This README provides a comprehensive overview of the project, including the structure, installation steps, usage instructions, and results of the model evaluations. If you have any questions or need further details, feel free to reach out!
Contributing
Contributions are welcome! Please read the CONTRIBUTING.md for guidelines on how to contribute to this project.

License
This project is licensed under the MIT License - see the LICENSE file for details.



## Contributing
Contributions to this project are welcome. To contribute:
1. Fork the repository.
2. Create a new branch for your feature (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Authors
- Bharath Gajula

## Acknowledgments
Special thanks to all contributors and those who provided feedback and suggestions to enhance the functionality and accuracy of the system.

---

This detailed README should provide a comprehensive guide to setting up, understanding, and contributing to the project, including how the system processes data and evaluates its performance. Adjust paths and specific implementation details as necessary to match your actual project setup.
