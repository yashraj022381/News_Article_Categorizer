# News_Article_Categorizer

 1. 📰 Project Overview
    
    - This project implements a Natural Language Processing (NLP) solution to automatically classify news articles into             predefined categories. It uses a machine learning approach, specifically the Multinomial Naive Bayes classifier,              trained on a corpus of news data.

    - The model is built to distinguish between five major news categories: 'entertainment', 'business', 'sport', 'politics',       and 'tech'.
   
 2. ✨ Features
  
    - Data Preprocessing: Includes custom functions for cleaning text data, such as converting text to lowercase,                   tokenization, removing punctuation, and filtering out English stopwords.

    - Feature Engineering: Explores two distinct text vectorization methods for comparison:

       - Bag-of-Words (BoW) using CountVectorizer.

       - Term Frequency-Inverse Document Frequency (TF-IDF) using TfidfVectorizer.

    - Machine Learning Model: Utilizes the Multinomial Naive Bayes classifier, which is highly effective for text                   classification tasks.

    - Model Evaluation: Performance metrics are generated using classification_report to assess the model's accuracy,               precision, recall, and F1-score for each category.

 3. 💻 Technologies Used
    
  - The project is developed using Python and relies on the following key libraries:

    - Python 3.x

    - pandas and numpy for data manipulation.

    - nltk (Natural Language Toolkit) for text preprocessing (tokenization and stopwords).

    - scikit-learn for machine learning:

      - CountVectorizer and TfidfVectorizer

      - MultinomialNB

      - train_test_split and classification_report.
     
  4. 🛠 Installation
     
     (i) Prerequisites
        - You need to have Python installed on your system.
        - Steps
          
      a) Clone the repository:

        Bash

       git clone https://github.com/YourUsername/YourRepoName.git cd YourRepoName

       b) Install dependencies:

        Bash

        pip install pandas numpy nltk scikit-learn

       c) Download NLTK resources:
          The notebook requires the 'punkt' and 'stopwords' resources from NLTK. You can download them by running the                   following commands in a Python environment:

        Python

        import nltk
        nltk.download('punkt')
        nltk.download('stopwords')

       d) Data:
          Ensure the dataset file, named bbc_data.csv, is present in the project directory, as the notebook is set to read              from it directly.

     (ii) 🚀 Usage
         The entire workflow, from data loading and preprocessing to model training and evaluation, is contained within                the News_Article_Categorizer.ipynb Google Collab Notebook.

       a) Start Collab:

        Bash

        collab notebook News_Article_Categorizer.ipynb


        b) Run Cells: Execute the cells sequentially to:
          - Load and explore the data.
          - Define the text preprocessing function.
          - Create the Bag-of-Words and TF-IDF feature matrices.
          - Train and evaluate the Multinomial Naive Bayes model using both sets of features.
    
        c) Test with Custom Text: The final cells demonstrate how to classify a new, unseen article:

        Python
     
     custom_text = "Artificial intelligence is revolutionizing the tech industry, with companies racing to develop the next         big innovation."

   5. 📊 Results and Evaluation
      
   - The notebook evaluates the performance of the Multinomial Naive Bayes model using both vectorization techniques (BoW          and TF-IDF) on the test set.

     (Note: You would typically include the actual performance metrics here once the notebook is run.)
