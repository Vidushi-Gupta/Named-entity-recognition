# Named-entity-recognition

## Abstract

Named Entity Recognition (NER) - also known as Entity Recognition or Entity Extraction - is a natural language processing (NLP) technique that automatically identifies and classifies named entities in text into predefined categories. An entity can be a person's name, organization, location, time, amount, monetary value, percentage, etc. An example of how named entity extraction NER works. The highlighted entities are WeWork, Adam Neumann, Manhattan and $37.5 million With named entity recognition, you can extract key information to understand what the text is about, or simply use it to gather important information and store it in a database.
NER scans all text and identifies named entities: it identifies sentence boundaries in a given document based on capitalization rules. Identifying sentence boundaries will help NER to find and extract relevant information from documents for subsequent steps. Categorize entities into predefined categories: In order to tokenize words or phrases, entity categories such as place, person, event, time, organization, etc. must be clearly defined. The entity extraction model can then be trained with predefined categories so that it can recognize entities such as people, places, and organizations in the raw text.

## Motivation

NER is a method that helps in recognizing the entities among a big pool of data, thereby it has many use cases. The motivation of this project was to build a NER model which has various use cases. The aviation industry, customer support, etc. use NER to differentiate between names of locations, people, dates, all of which are entities. Thus, in order to gain some industrial exposure, the following project has been implemented. 

## Limitations of existing methods

Currently, the task of identifying transliterated entities is dominated by NER models, which develop an algorithm to tag foreign language or transliterated entities, or use metadata from Wikipedia, such as cross-wiki links, article categories, and cross-language links, or other parallel Non-English language becomes speech data. In the first approach, the model is trained on multilingual Wikipedia text, and NER for non-English and/or transliterated words is predicted based on the trained model. This approach has limitations because articles can have different content depending on language: some countries censor certain topics, or articles on controversial topics like Crimea can have different content depending on language. Given these differences, training with cross-language Wikipedia articles may not yield accurate results. Automatic translation seems like a possible solution to this approach, but it can also introduce inaccuracies.

The second approach, in which the NER model is trained with annotated data, seems to be more reliable, but a marked corpus is clearly not available for transliterated entities from Arabic to English. Furthermore, for general Arabic, most labeled corpora contain modern web content where place names and historical names of cities (often found in Lorimer's gazetteer) may be underestimated. To address these limitations, in this project we annotate Lorimer's Gazetteer and create a large amount of training data to label historical transliterated NEs from Gazetteer. This annotated dataset may further benefit other projects dealing with historical or non-historical texts containing transliterated words.

## Proposed method with architecture/flow diagram

![image](https://user-images.githubusercontent.com/55969597/162585929-e3b15d8b-70a1-4f46-9441-4858591dd377.png)

## Modules with description

- Acquiring Dataset
- Extracting mappings : Features and Labels
- Extracting data sequentially
- Identifying the best fit model
- Training the model
- Testing the model
- Evaluating + feedback the model

## Screenshots

![image](https://user-images.githubusercontent.com/55969597/162586035-713e1a2a-3e54-446c-b43c-3c6b3782be64.png)

## Conclusion

Thus, the entities have been identified from the text. With an improved GPU and an increased number of epochs, the accuracy of the neural network can be improved. This can be implemented in almost every industry which generates a high volume of textual data. 

## Contributors

- [Vidushi Gupta](https://github.com/Vidushi-Gupta)
- [Abhimanyu Bhadauria](https://github.com/Mnayu)

