# Text Classification using the MBTI Dataset

## Project Brief

This project utilizes the Myers-Briggs Type Indicator (MBTI) dataset to explore text classification techniques. The MBTI, developed by Katharine Cook Briggs and her daughter Isabel Briggs Myers, categorizes individuals into 16 distinct personality types based on four principal psychological functions: sensation, intuition, feeling, and thinking. Despite questions about its validity, the MBTI remains widely used across various domains. Our goal is to identify patterns in writing styles associated with MBTI types, assessing the test’s utility in analyzing, predicting, or categorizing behavior.

## Dataset

The dataset comprises approximately 8,000 entries, each including:
- **Type/Class Label:** A 4-letter MBTI type code.
- **Text:** Posts made by the individual, separated by "|||" (three pipe characters).

We use this data to train a classifier that predicts personality types based on textual input, purely for educational purposes related to text classification.

## Classifier Design and Evaluation


## Classifier Design and Evaluation

### Design
- **Classifier Type:** Combination of BERT and traditional machine learning models designed for text classification.
- **Architecture:** 
  - **BERT Model:** We utilize a pre-trained BERT model for feature extraction, taking advantage of its deep learning capabilities to understand the context within the text data.
  - **Traditional ML Models:** Post-feature extraction by BERT, we employ traditional machine learning classifiers (such as Logistic Regression, SVM, and Random Forest) to categorize text into one of the 16 MBTI personality types. This hybrid approach leverages both deep learning and traditional statistical methods for effective classification.

### Cross-Validation and Performance Measures
- **Methodology:** We implement five-fold cross-validation to validate the classifier's effectiveness across different subsets of data.
- **Performance Metrics:** The classifier is evaluated using accuracy, recall, precision, F1 score, and confusion matrices. This comprehensive assessment helps gauge both the overall and individual performance aspects of the model.

## Results

We provide detailed results from each fold of cross-validation, including performance metrics and analyses. Insights into how the combined use of BERT and traditional models impacts classification effectiveness are thoroughly documented.

## Reproducing Results

To replicate our findings, follow these steps:

1. **Environment Setup:**
   - Ensure Python 3.8+ is installed.
   - Install dependencies: `pip install -r requirements.txt`.

2. **Data Processing:**
   - Use scripts in the `data_preparation` folder to format and partition the MBTI dataset.

3. **Model Training and Evaluation:**
   - Execute the Jupyter Notebooks:
     - `BERT_NLP_3.ipynb` for setting up the BERT model and integrating it with traditional classifiers.
     - `NLP_ML_Models_Assignment3.ipynb` for conducting the cross-validation and generating performance metrics.

4. **Viewing Results:**
   - Detailed performance analysis is available within the notebooks or through additional scripts in the `results_visualization` folder.
## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
