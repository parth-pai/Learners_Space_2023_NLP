## WnCC Learner's Space 2023 - Natural Language Processing.

In the *final project* of Learner's Space, I built a Language Translation model (from English to Italian) and fine-tuned it for better performance of the model. 
## This is my link to the Google drive folder of pre-trained model : https://drive.google.com/drive/folders/135ksdaONW43-_PxECt9VUlj5AK2ryYQm?usp=sharing

## Dataset:
I used enimai/MuST-C-it dataset from Huggingface which has both sentences in English and their Translation in Italian. It has around 250k rows. Hence it was a suitable dataset to train from.

Link: https://huggingface.co/datasets/enimai/MuST-C-it

## Model Used : 
I used Helsinki-NLP/opus-mt-en-it model from Huggingface to see translation in practice from the datasets

Link: https://huggingface.co/Helsinki-NLP/opus-mt-en-it

I used "sacrebleu" scoring method to evaluate the model for fine-tuning. 

## Unique Challenges Faced:
Choosing the dataset was a task on itself because some of them had way too many rows(~4M+) which couldn't be handled by colab and some had way too less rows (~10k) which would not be suitable for training. Also even though the code I had written was correct, the trainer wasn't getting pushed to Huggingface hub. That's why I later uploaded the model to google drive and operate further.
