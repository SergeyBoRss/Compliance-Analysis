dataset.json - First created dataset for structuring data;
fixed_dataset.json - Datset with type "promt - response" and response is predicted text;
label.json - Dataset with type "promt - response and response is label of classification;
output.json - Dataset like dataset.json, but it have alone string for every object;

Idea: use a pre-trained LLM Mistral 7B 0.3v model to generate Description and Difference text.
We strip away the embeddings on one of the last layers of the LLM to train our own full-link nlp classification model. 
We get the classification label type from the full-link model and the generated text. 
