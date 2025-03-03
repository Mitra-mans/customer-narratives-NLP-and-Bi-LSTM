NLP-Based Customer Narrative Classification Using Bi-LSTM

This project uses Natural Language Processing (NLP) and machine learning to analyze and classify customer complaints into predefined product/service categories. The aim is to help businesses identify key customer pain points and enhance satisfaction.

Project Workflow
1. Exploratory Data Analysis (EDA) and Preprocessing

    Objective: Prepare the data and uncover insights about customer complaints.

    Steps:
        Removed irrelevant columns and handled missing or empty entries.
        Visualized the distribution of products and narrative lengths using bar plots and histograms.
        Conducted text preprocessing:
            Removed punctuation, numbers, contractions, and stopwords.
            Applied tokenization and lemmatization.
        Identified the most common words and visualized them with bar plots and word clouds.
        Addressed class imbalance through oversampling.

    Results:
        Found a high volume of complaints in credit reporting.
        Balanced the dataset effectively for improved model training.

2. Bi-LSTM Model Development

    Objective: Build an advanced deep learning model for text classification.
    Model Details:
        Text preprocessing: Tokenized, padded, and embedded narratives.
        Architecture:
            Two Bidirectional LSTM layers for learning sequential patterns.
            Dropout layers to prevent overfitting.
            Dense layer with softmax activation for classification.
        Training:
            Loss function: Sparse Categorical Cross-Entropy.
            Optimizer: Adam.
            Dataset split: 80% training, 20% validation.
    Results:
        Achieved ~93% accuracy, with strong Precision, Recall, and F1-Score across all categories.

3. Comparison with Traditional Classifiers

    Objective: Benchmark Bi-LSTM against simpler machine learning models.
    Models:
        Naïve Bayes Classifier: Struggled with imbalanced and complex datasets.
        Random Forest Classifier: Performed better but fell short of Bi-LSTM.
    Results:
        Bi-LSTM demonstrated superior accuracy and better handling of narrative complexity.
