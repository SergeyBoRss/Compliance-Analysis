dataset.json - First created dataset for structuring data;
fixed_dataset.json - Datset with type "promt - response" and response is predicted text;
label.json - Dataset with type "promt - response and response is label of classification;
output.json - Dataset like dataset.json, but it have alone string for every object;

Идея: использовать предобученную LLM Mistral 7B 0.3v модель для генерации текста Description и Difference. 
Мы отнимаем эмбединги на одном из последних слоев LLM для обучения собственной полносвязной модели nlp классификации. 
Получаем тип метки классификации из полносвязной модели и сгенерированный текст. 
