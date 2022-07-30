# Predicting Russion Trolls Types by Interactions' Structure and Content

We present a ML-framework to predict twitter user's troll type () based on their interactions with known trolls.
The data is based on the IRA tweets and interactions analyzed by [Linvill and P. L. Warren](https://misinforeview.hks.harvard.edu/article/engaging-ira-coordinated-information-operation/) and others.

We propose a framework, where from a known troll, we are able to classify all other users it interacted with (on twitter) as trolls (and their type)or not, with high accuracy.

The framework employs two main concepts: (1) The structure of an interaction (based on a generated interactions graph) is informative to the actors (in this case twitter users) themselves. 
(2) The content of the interaction itself (in this case, the content of the tweet reply or quote) is also informative. These two concepts combined yield powerfull predictions
and enable future researchers to "grow" a trolling network from a single "seed" user.

We utilize two embeddings caluclation techniques as features - Node2Vec using [RandomWalk](https://dl.acm.org/doi/pdf/10.1145/2939672.2939754?casa_token=NIU75TQ2tmAAAAAA:teK2y7swRrlJ6IcIjqlS5rfqbgb77kueLCR5jiBZw4C52JpQIQHJjzl1gVWvD3mfxgmi8VE0tylw0nY)
and word embeddings using [BERT](https://arxiv.org/pdf/1810.04805.pdf&usg=ALkJrhhzxlCL6yTht2BRmH9atgvKFxHsxQ). 

The entire process and a comprehensive report about the framework and results can be found in the "report.pdf" found in this repository.

Notebooks found in this repository were implemented and meant for use in google colab. 
They are divided into the report sections://
Raw IRA data preprocessing and initial exploration - 'Data_NLPSD.ipynb'

Twitter API scraping for additional users information - 'TwitterAPI For Users Description.ipynb'

EDA Exploratory Data Analysis (including graph construction) - 'DataExploration.ipynb'

Content and graph embeddings - 'node2vec.ipynb'

Deep Neural Network, design, implementation, training and testing - 'Clustering_by_embeddings_and_Modeling.ipynb'

Sensitivity Analysis - 'Sensitivity_Analysis.ipynb'


For any question/suggestion, please feel free to approach us @:
- Yishaia Zabary - yshaayz@gmail.com
- Dan Avraham - dan.avraham23@gmail.com
- Yizhak Veisman - aitzikvais@gmail.com

This code is open-source and free for all to use under the GPL V3 license.
![GPLV3](https://www.gnu.org/graphics/gplv3-with-text-136x68.png)

