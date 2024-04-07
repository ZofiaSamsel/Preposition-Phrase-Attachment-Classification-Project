
# Preposition Phrase Attachment Classification Project

## Overview

The Preposition Phrase attachment problem involves determining whether a preposition in a sentence is attached to a verb or a noun. This ambiguity can lead to confusion for readers. For example, in the sentence "San Jose cops kill man with a knife," it's unclear whether the man or the cops were holding the knife. Resolving this ambiguity requires understanding the syntax and semantics of the sentence.

In this project, we aim to classify prepositional phrases (PP) as attached to either a verb (V) or a noun (N). We'll explore various classification models and evaluate their performance using different features and techniques.

## Dataset

We utilize a dataset containing examples of prepositional phrases along with their correct attachments (N or V). The dataset consists of 25,858 samples.

### Step 1: Data Exploration

- Examined the dataset statistics.
- Inspected random samples to ensure correct labeling.
- Analyzed the distribution of examples per group (N and V).
- Explored the distribution of prepositional phrases and their attachments.

### Step 2: Feature Engineering

- Created features including single items, pairs, triplets, and quadruples to capture linguistic aspects.
- Considered advanced features such as corpus level information and distance metrics.

### Step 3: Model Selection and Evaluation

**Classifiers Explored:**
- Support Vector Machine (SVC)
- K-Nearest Neighbors (KNN)
- Random Forest
- Complement Naive Bayes
- Multinomial Naive Bayes

**Vectorization Methods:**
- CountVectorizer
- TfidfVectorizer

**Evaluation Metrics:**
- Accuracy Score
- GridSearchCV for hyperparameter tuning

## Results and Insights

- Explored different vectorization methods and classifiers.
- Utilized GridSearchCV for hyperparameter tuning.
- Evaluated models using both accuracy and cross-validation scores.
- Achieved test accuracy scores ranging from 82% to 83%.

## Future Directions

- Explore additional features and techniques to improve classification performance.
- Experiment with ensemble methods and deep learning models.
- Incorporate external linguistic resources like WordNet or word embeddings for enhanced feature representation.
- Further analyze misclassified examples to identify patterns and improve model performance.

## How to Open the Project

To open and explore the project:

1. Clone the repository from GitHub using the following command:
   ```
   git clone https://github.com/your_username/preposition-phrase-attachment-classification.git
   ```

2. Navigate to the project directory:
   ```
   cd preposition-phrase-attachment-classification
   ```

3. Open the project files in your preferred Python development environment, such as Jupyter Notebook, PyCharm, or VS Code.

4. Install the required dependencies by running:
   ```
   pip install -r requirements.txt
   ```

5. You can now run and modify the project code to further analyze the preposition phrase attachment classification task.

## Conclusion

The project demonstrates the process of tackling the Preposition Phrase attachment problem through data exploration, feature engineering, model selection, and evaluation. While achieving good accuracy scores, there's still room for improvement through experimentation with advanced techniques and incorporating external linguistic resources. This project serves as a foundation for further research in natural language processing and text classification tasks.
