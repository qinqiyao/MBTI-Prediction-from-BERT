# MBTI-Prediction-from-BERT

Data was collected through the Personality Cafe forum, as it provides a large selection of people and their MBTI personality type, as well as what they have written.

This dataset contains 8675 rows of data, on each row is a person:

Type (This persons 4 letter MBTI code/type)

A section of each of the last 50 things they have posted (Each entry separated by "|||" (3 pipe characters))


Training Set: 6940
Testing Set: 1735

Regex is used to detect special characters like '@,emojis' etc. from the posts, remove stopwords and punctuation, convert the text to lowercase and stemming to extract the root of words. 

BertTokenizer is responsible for tokenizing and encoding raw text into token IDs required by the BERT base model. The maximum input length for BERT is 512 tokens:

Weighted Fine-tuned BERT (109,494,544 parameters to be trained)

   
