# Natural Language Processing in Hindi
- State of the Art Hindi Language Model and Classifier
- Language Model trained on Hindi Wikipedia Articles
- Classifier trained on Hindi Movie reviews Dataset
- [Make your own Hindi Predictions using Language model playground](https://colab.research.google.com/github/mananm98/Hindi-Text-Classification/blob/master/Language_Model_Playground.ipynb)

## Datasets
- [Hindi Wikipedia Articles Dataset](https://drive.google.com/file/d/11aZeRC0uYQz6ScvmHQucfn7fwryqxPUd/view?usp=sharing)
- [Hindi Movie Reviews Datset](https://www.kaggle.com/disisbig/hindi-movie-reviews-dataset)

### Wikipedia Articles Dataset
- The Hindi Wikipedia Articles was created using wikipedia dump file, the **latest** file containing all the Hindi articles and pages can be downloaded from https://dumps.wikimedia.org/hiwiki/latest/hiwiki-latest-pages-articles.xml.bz2

- Wikipedia Articles Dataset can be built for any language with the latest Articles, by replacing the **WP-Code** of the chosen language in this URL `https://dumps.wikimedia.org/{hi}wiki/latest/{hi}wiki-latest-pages-articles.xml.bz2`. Here, **hi** is the code for Hindi Language.

- **WP-code** is the Language code used by wikipedia to refer to a language. The list of codes can be found [here](https://en.wikipedia.org/wiki/List_of_Wikipedias)

- Hence, we can build Language Models for other languages very easily using Wikipedia data

### Hindi Movie Reviews Dataset
- This dataset was downloaded from this amazing [repo](https://github.com/goru001/nlp-for-hindi) by **Gaurav Arora**. Check out his [github](https://github.com/goru001), he has done great work for other Indian languages as well.

## Wikipedia Language Model predictions
The Language Model Makes Some Cool Predictions ✨

![predictions](https://github.com/mananm98/Hindi-Text-Classification/blob/master/images/Screen%20Shot%202020-05-27%20at%2014.03.11.png)

- After pretraining, the Hindi Language Model was fine tuned on Hindi Movie Reviews dataset. Then the encoder of fine tuned Language Model was used to further train the Hindi Text Classifier. This method of training a classifier is called [ULMFIT](https://arxiv.org/abs/1801.06146) and it was introduced by Jeremy Howard and Sebastian Ruder.

## Results 
| Model  | Accuracy on Test Set |
|--------|----------------------|
| ULMFIT | 62.27%               |

## Downloads
- [Hindi-Wikipedia-Language-Model](https://drive.google.com/file/d/1qPP6hGKS1CxBb2ZtVVASDLUQz_qa5y1i/view?usp=sharing)
- [Hindi-Text-Classifier-Positive|Neutral|Negative](https://drive.google.com/file/d/1nhws0wZLihhVehmqQHT-B38V17FJp9eS/view?usp=sharing)  
Note : The language model and classifier are fastai learner objects, they will work with the [fastai library](https://docs.fast.ai/basic_train.html#Learner.load)

## Run in Colab
- [Hindi Text Classification Notebook](https://colab.research.google.com/github/mananm98/Hindi-Text-Classification/blob/master/Hindi_Text_Classification.ipynb)
- [Language Model Playground](https://colab.research.google.com/github/mananm98/Hindi-Text-Classification/blob/master/Language_Model_Playground.ipynb)

