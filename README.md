# Sentiment-Analysis-in-Political-News-Coverage
This project is part of a research paper titled "Utilizing Pre-Trained Models for Sentiment Analysis in Political News Coverage". 

The goal of this project is to demonstrate the use of a pre-trained DistilBERT model for classifying political news headlines into three sentiment categories: positive, negative, and neutral.  

### Key Steps:
1. Dataset: The Political News Headlines dataset (`uci-news-aggregator.csv`) from Kaggle link of dataset (https://www.kaggle.com/datasets/uciml/news-aggregator-dataset?utm_source=chatgpt.com) is used. The dataset contains news headlines and associated categories (Business, Tech, Entertainment, Medicine).  
2. Preprocessing: Only the `TITLE` (headline) and `CATEGORY` columns are used. A human logic mapping converts categories into sentiment labels:  
   - `b` (business) → Neutral  
   - `t` (technology/science) → Neutral  
   - `e` (entertainment) → Positive  
   - `m` (medicine/health) → Negative  
3. Model: A pre-trained DistilBERT model from Hugging Face Transformers is fine-tuned for sentiment classification.  
4. Evaluation: Model performance is assessed using accuracy, precision, recall, F1-score, and confusion matrix visualization.  
5. Inference: Example political headlines are tested to verify the model’s predictions.  

### Outcome:
This notebook shows how pre-trained NLP models can effectively analyze political news coverage, providing insights into sentiment trends across domains. The implementation reflects the methodology and results discussed in the research report.

