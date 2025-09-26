# Human-Activity-Recognition-with-Feature-Reduction
Built a Human Activity Recognition model using the UCI Smartphone dataset. Trained a Naive Bayes baseline on 561 features (73% accuracy) and applied K-Means feature reduction to 50 features, improving accuracy to 81% while cutting training time from 0.37s to 0.01s. Implemented with Python, scikit-learn, Pandas, NumPy, and BeautifulSoup.

## Dataset

The project utilizes the "Human Activity Recognition Using Smartphones" dataset from UCI Machine Learning Repository. This dataset contains sensor readings from smartphones worn by individuals performing various activities like walking, standing, sitting, etc.

## Methodology

1. **Data Loading and Preprocessing:** The dataset is downloaded, loaded, and preprocessed. This involves encoding class labels and scaling features using StandardScaler.
2. **Baseline Model:** A baseline model is trained using all features and a Naive Bayes classifier. Performance metrics and training time are recorded.
3. **Feature Reduction with K-Means:** K-Means clustering is applied to reduce the number of features. Features are clustered based on their similarity, and representative features from each cluster are selected.
4. **Model with Reduced Features:** A new model is trained using the reduced feature set and the same Naive Bayes classifier. Performance and training time are compared with the baseline model.

## Results

The results demonstrate the impact of feature reduction on model performance and training time. The reduced model achieves comparable accuracy to the baseline while significantly reducing training time and the number of features used.

## Usage

1. Clone the repository.
2. Install the required libraries: `pip install scikit-learn pandas requests beautifulsoup4`
3. Run the Jupyter Notebook `main.ipynb` to execute the code.

## Contributing

Contributions are welcome! Feel free to open issues or pull requests for bug fixes, enhancements, or new features.

## License

This project is licensed under the MIT License.
