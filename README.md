📝 Project Overview
This project performs binary sentiment classification on IMDb movie reviews using a logistic regression model combined with pre-trained Word2Vec embeddings. It demonstrates how classical machine learning techniques can achieve strong performance on real-world NLP tasks using minimal computational resources.

⚙️ Technologies Used
Google Colab / Python 3.11

nltk – for tokenization and stopword removal

gensim – for loading Google News Word2Vec embeddings

scikit-learn – for logistic regression and evaluation metrics

datasets – for downloading IMDb reviews

numpy, pandas – for data manipulation

matplotlib / tqdm – for visualization and progress display

📂 Project Structure
├── imdb_sentiment_analysis.ipynb   # Main Colab notebook with all code
├── sample_output.png               # Evaluation bar chart (optional)
├── README.md                       # Project documentation
🔄 How to Reproduce
Open the notebook in Google Colab. link: https://colab.research.google.com/drive/1SaFGdAC8ktC5ggZXZ3ETpnhGcltVFJUO?usp=sharing

Run all cells in order (no GPU required).

The model will preprocess 5,000 IMDb reviews, generate sentence embeddings, train a classifier, and output performance metrics and visualizations.

Note: The Word2Vec model (word2vec-google-news-300) will be downloaded (~1.5GB) via gensim.downloader on first run.

📊 Results Summary
Metric	Score
Accuracy	84.6%
Precision	86.9%
Recall	82.5%
F1 Score	84.6%

The classifier demonstrates strong overall balance and is especially effective at minimizing false positives.

⚠️ Limitations
Word embedding averaging loses word order and context.

Sentences with mixed tone or negations may be misclassified.

Transformer-based models (e.g., BERT) would likely perform better on nuanced data.

📁 License
This project is for academic and educational use only. No commercial reuse permitted without explicit permission.
