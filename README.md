# Topic Modeling for Research Software
This project aims to provide different topic models to analyze research software. On this note this NLP tool is used to process different papers abstracts and the README files corresponding to their Github repository. 
This project was done as a Master Thesis at UPM. 

## Abstract
Currently, the amount of daily publications in different fields of Machine Learning
makes it impossible for researchers to be up to date and even to find what they’re
looking for in a reasonable amount of time. This problem can be extended also for
software developing, where reusing already developed code could save them up much
research time.

In this thesis, we propose different methods for processing a large number of papers
along with their software, based on abstracts obtained from Papers With Code and
their corresponding README files, in order to save researchers time and facilitate
software adoption . This approach relies on topic modeling to extract the main topics
present and assign them to the different publications without having to read them
all. We use three different algorithms to find the most coherent topics. LDA is the
algorithm most used when modelling topics within text, and has proven to be effective
although it also has some limitations . To cover its limitation on working with docu-
ments of short length we also propose applying BTM, which was specifically designed
for these types of text . LDA can also find problems to handle semantic relationships.
For this we used BERTopic, which uses the hability of pretained language models to
find better and contextualized text representations.

Results corroborate the assumed effectiveness of LDA, while highlighting the influ-
ence of hyperparameter tuning. BERTopic also provided coherent and interpretable
topics. Generally, we conclude that our models effectively identify most of the top-
ics and could be useful for future topic search implementations or recommendation
systems.

## Contents
- The data collection process can be found in the folder *collection*.
- The preprocess of both abstracts and README files is hold in *preprocess*.
- In *models* the different models built to answer both research questions are found.
- In *results* different csv files keep the hyperparameter tuning results of all models.
- TFM_Maria_Ayuso is the Master Thesis document associated with this repository.

## Data
- The data used in this study was obtained through the Papers With Code platform. To reproduce the same results, the same data can be downloaded in : <https://doi.org/10.5281/zenodo.6788250>
- The data obtained both after web scrapping and after the preprocess can be found in : <https://doi.org/10.5281/zenodo.6788314>
