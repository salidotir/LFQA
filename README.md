

# Rpository Structure:
```
- 📦 ....
  |- 📄 README.md                        #Guide file
  |- 📂 data                             #Here you can see dataset link.
  |- 📂 notebooks                        #Here you can see jupyter files which should be run on Google Colab.
     |- 📂 1_Preprocessing                 #Here you can run first preprocessing tasks on dataset
     |- 📂 2_Models                        #Here you can see three models; BART, RAG, LLAMA, respectively. You can run each you want.
     |- 📂 3_Content_Classification        #Here you can  see second task of problem using Logistic Regression and NiveBayes
     |- 📂 4_Results                       #Here you can see the genereated answers and Rouge scores obatined of Model_3
     |- 📂 5_Ui_Interface                  #Here you can see UI Interfaces for asking your questions
 |- 📂 report                           #Here you can see a complete report of what we have done.


```

# Project Detail

**Problem**:
Long Form Question Answering & Generated Content Detection

**Goal**:
1_To create an NLP model that can produce detailed and accurate long-form answers for questions in the ELI5 dataset.
2_To Generate Content Detection

# Dataset Detail:
The dataset utilized in this project is a subset of the "Explain Like I'm Five" [ELI5 dataset](https://huggingface.co/datasets/rexarski/eli5_category), which originates from a popular Reddit forum where complex concepts are explained in simple terms.
The full ELI5 dataset comprises over 270,000 question and answer pairs, with each pair containing a detailed explanation suitable for a layperson. The questions cover a broad range of topics, making the dataset a rich resource for training models that require a deep understanding of diverse subjects.

# Dataset Structure: 
DatasetDict({
    train: Dataset({
        features: ['q_id', 'title', 'selftext', 'category', 'subreddit', 'answers', 'title_urls', 'selftext_urls'],
        num_rows: 91772
    })
    validation1: Dataset({
        features: ['q_id', 'title', 'selftext', 'category', 'subreddit', 'answers', 'title_urls', 'selftext_urls'],
        num_rows: 5446
    })
    validation2: Dataset({
        features: ['q_id', 'title', 'selftext', 'category', 'subreddit', 'answers', 'title_urls', 'selftext_urls'],
        num_rows: 2375
    })
    test: Dataset({
        features: ['q_id', 'title', 'selftext', 'category', 'subreddit', 'answers', 'title_urls', 'selftext_urls'],
        num_rows: 5411
    })
})



# **Guide to use**:
You can run each jupyter file using [colab](https://colab.research.google.com/notebooks/) or [Kaggle](https://www.kaggle.com/).
N.B . The fine-tuned models in each file have been linked using our dirves.




