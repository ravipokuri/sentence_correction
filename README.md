Introduction:
As we all know,we are in the 21st century which is just a digital book.
Here people express themselves through various social networks like
facebook,instagram,whatsapp etc. we will use the data from these
social networks and preprocess them with some nltk tools and try to
apply them to nlp systems to predict any criminal activity that are
hazardous to society. Not only this example we can also use them in
predicting the winner in elections,also in psychometric assessment
and what not, we can use that data to do lot many things that benefit
society. But the main problem we are facing is now a days people are
using short cut language in expressing themselves. For example how
about you as hbu and how are you as hru which is corrupted form of
the actual english.they might not be that much useful information in
that a machine learning or deep learning model can get cause these
models are not designed for using the corrupted language.





Business Problem:
Our main task here is to convert those corrupted text to normal
english by preserving the context's meaning. after that we can give
them to the NLP systems so that they work fine while doing their job.





Source of Data Set:
http://www.comp.nus.edu.sg/~nlp/sw/sm_norm_mt.tar.gz




Data Overview:
There are about 2000 data points in that data set. Data is spread like
shown below. First there is sms text from social media and after that
the actual english text preserving the context meaning of above sms
text followed by the chinese translation of the english text. We are
using only sms text and english text for our purpose. We avoid chinese
translation translation because machine translation is not part of our
research paper.




![data](https://user-images.githubusercontent.com/48234359/140685143-ea67540c-bef4-4a96-8742-d7f81c286501.png)




Here we have used multiple models like:
1.For embeddings used Character level glove embeddings,word level glove embeddings,Character level fasttext embeddings, word level fasttext embeddings and to capture the sequence information used LSTM.
2.At the time of inference,used beam search for effectively predicting most probable word.
3.LSTM with glove word embedding and Bahadanau Attention mechanism.



