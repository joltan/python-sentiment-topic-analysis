# python-sentiment-topic-analysis

## OBJECTIVE
This project compares user perception of WhatsApp, Discord and Signal by extracting and analysizing user reviews using sentiment analysis (nltk library) and topic modelling using LDA.

## DEPENDENCIES
Run the following lines to install the dependent libraries before testing the notebook.
!pip3 install pandas scikit-learn vaderSentiment nltk wordcloud spacy
!python -m spacy download en_core_web_sm

## APPROACH
1. By using Beautiful Soup library, we created a 'reviews' dataframe by scraping all reviews for each of Whatsapp, Signal, and Discord from Trustpilot.
2. Only English reviews were selected, resulting in 439 Whatsapp reviews, 17 Signal reviews, and 650 for Discord.
3. All reviews were cleaned where punctuations were removed using standard Python built-in functions, using code from: https://github.com/hakimkhalafi/trustpilot-scraper/blob/master/clean.ipynb
4. spaCy model is often regarded as the most accurate and effective for lemmatization, which includes removing irrelevant words through a combination of lemmatization and part-of-speech tagging.  Since it is widely used in various natural language processing tasks, including sentiment analysis, we have chosen SpaCy and English language model ('en_core_web_sm') for stemming step.
English language model (en_core_web_sm).
5. Lastly, tokenization was conducted before the final Sentiment Analysis from Python's NLTK library.
