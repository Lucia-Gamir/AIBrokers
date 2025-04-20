🧠 AIBrokers – Alert System
This project was developed as part of the Deep Learning and Natural Language Processing course. Its main goal is to build an automated alert generation system to support investment decisions by combining text analysis and image processing.

📚 PROJECT OVERVIEW
AIBrokers is a system that takes textual and visual input, analyzes the content using Named Entity Recognition (NER), Sentiment Analysis (SA), and Image Captioning models, and then generates a recommendation on whether to invest in a company based on the extracted information.

⚙️ PROJECT STRUCTURE & NOTEBOOKS
- Data files:
    - finer_ord_*.csv: CSV file. Each row has the document label, token, identifier and sentence identifier separated with comas.
    - finer_*_data.json: JSON file. Each object has the sentence and a list of its entities. 
    - sentiment_*.csv: CSV file. Each row has the sentence and its sentiment.  

- Embeddings: 
    - AIBrokers_Bert_Embeddings.ipynb: Initial embedding experiments using BERT.
    - AIBrokers_Compared_Embeddings.ipynb: Embedding comparison between Glove, Word2Vec and KeyEyed Word2Vec was selected as the final approach.

- NER:
    - AIBrokers_NER.ipynb: Training and evaluation of Named Entity Recognition models.

- SA: 
    - V1_SA_Bert: First experiment with bert embeddings. 
    - V1_SA_w2v: First experiment with word2vec embeddings. 
    - AIBrokers_SA.ipynb: Training and evaluation of Sentiment Analysis models.

- Alert Generation & Image Captioning:
    - AIBrokers_Alert_Generation.ipynb: Main notebook. Integrates the best NER and SA models to generate investment recommendations based on textual and visual input. Includes an image captioning module to enrich the final output.

🔍 USED TECHNOLOGIES
Python 3
Jupyter Notebooks
spaCy
Gensim (Word2Vec)
Hugging Face Transformers (for BERT)
NLTK / TextBlob (for Sentiment Analysis)
TensorFlow / PyTorch (depending on model)
OpenCV / PIL (for image processing)
CLIP / BLIP / similar (for image captioning)

🧪 HOW TO USE
Open and run AIBrokers_Alert_Generation.ipynb.
Provide a text and image input in the last cell.

The system will return:
    Extracted entities (NER)
    Sentiment classification (SA)
    A generated caption for the image
    An investment recommendation based on all the above

✅ PROJECT STATUS
Embedding comparison and selection
NER and SA model training
Alert system integration
Working image captioning module


👥 AUTHORS
Hugo Albert Rodríguez de Miguel
Santiago Moreno Marín
Paloma Díez Amatriaín
Lucía Gámir Díaz