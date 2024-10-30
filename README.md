# NLP - Train itinary

This project's main goal is to suggest the best train itinary from an user prompt in France and in french. To achieve this, a frontend application using NextJS, coupled with a backend using Flask to directly channel the inferences from our AI models to the frontend.

This project was the occasion to train several models and pick the best one after a thorough benchmark. Each model was built with the previous one issues in mind, leading to 3 iterations:
- The first one is a simple Spacy model, akin to a RegEx with the goal of finding the departure and arrival thanks to its NER and the positionning in the sentence of the train stations.
- The second model is a 4000 classes classification BERT model, which was fine-tuned from a pretrained BERT from HuggingFace. Each class represents a train station.
- The third and forth ones are models working in tandem. A model was used as an NER, trained with IOB tagged sentences which goal is to tag each word in the sentence. The forth one is a classification model with 4 classes (departure, arrival, intermediary, none). These 2 models were fine-tuned from a pretrained BERT.

# Progress
The project is still ongoing, and a lot of things need to be finished. The end of this project is estimated to happen in January.

<!-- ## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here) -->


## Authors

- [@LeguyDany](https://www.github.com/LeguyDany)
- [@SanLamamba](https://github.com/sanlamamba)
- [@Mohamed-elhediKraiem](https://github.com/Mohamed-elhediKraiem)
- [@MokhtarBeny](https://github.com/MokhtarBeny)
