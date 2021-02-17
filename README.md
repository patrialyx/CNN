# Baseline-Model-on-image-sentiment-analysis
Sentiment analysis on multimodal media (memes)

Organised by SemEval-2019, an international workshop on Semantic Evaluation, the Memotion Dataset of 8K annotated memes with human 
annotated tags is released due to the task Memotion analysis. We set out to tackle the first task – Sentiment Classification, 
whereby the memes are to be classified into 5 categories: very positive, positive, neutral, negative, and very negative. 

Memes are a multimodal form, and can be decomposed into images and text. We can use Natural Processing Language techniques to tackle 
meme text and pretrained image models to detect the sentiment within images. These models are expected not to have high accuracies as
they are meant as baseline models to be compared with. 

In this analysis, we have experimented with the Bag-Of-Words technique as well as the state of the art bidirectional encoder BERT.
BERT was hypothesised to do better due as it analyses clauses without any specific direction, however, Bag-of-Words+Simple Multilayer 
Perceptron actually achieved better performance. Regarding image recognition, the VGG model was the only model which showed signs of 
improvement out of a handful of pretrained models tested.

Moving forward, For future works, a multimodal pipeline can be considered, combining the results of the best pretrained image 
classification model with the best-performing text classification models. Due to the lack of similarities between images under each label,
the most targeted feature that can be utilised is facial expressions, to obtain overall sentiment. However, it is also noted that the 
overall sentiment expressed by facial expression may differ from the overall sentiment which the author intends to express. 

