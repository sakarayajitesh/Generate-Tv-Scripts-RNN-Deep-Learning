# Generating Tv Scripts
Building a **Deep Learning** model which generates new TV scripts starting with a given word something like this :\
\
**Word** = "jerry"

```
jerry:

george: i think i have the same.

jerry: i mean, it's like you can get the money.

jerry:(to himself) what?

elaine: oh!

kramer:(to jerry) i think we have a big salad.

kramer: yeah.

jerry: i don't know.

jerry: well, you can't believe that.

george: i think you may have.

jerry:(to jerry) you know, i'm not gonna go. i'm going to the airport, i don't even know why i want.

jerry: what?

elaine: what is that?

jerry: you know. you can't believe it. it's like a sauna.

jerry: i know.

elaine: oh, no, you know, i was a good driver, and i have no idea.

george: oh, yeah. i don't want to know that i was a little bit...

jerry: what are you going to do?

george: i don't think so.

```


# Overview
The model uses RNNs to generates new TV scripts.

* **Network** :
  1) Embedding Layer 21388 (Vocabulary size + 1) -> 256 (Embedding size)
  2) LSTM 256 -> 600
  3) Fully Connected Layer 600-> 21387 (Vocabulary size)
  
* **Loss** : Cross Entropy 
* **Optimizier** : Adam
  

# Dependencies
* Python
* PyTorch
* Numpy
* Matplotlib


# Steps involved
1. Creating Lookup table
2. Batching the data
3. Building the Network
4. Setting hyperparameters
4. Training the model
5. Generating Text
