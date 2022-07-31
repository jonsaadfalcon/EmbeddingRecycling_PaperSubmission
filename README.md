# Embedding Recycling
## Datasets

To access our datasets for text classification and named-entity recognition (NER), please go to the folders titled `text_classification` and `ner` in the `data` folder of the [SciBERT](https://github.com/allenai/scibert/) repository. 

To access our datasets for question answering (QA), please access the TriviaQA and SQuAD datasets on HuggingFace at the following links:

- [TriviaQA](https://huggingface.co/datasets/trivia_qa)
- [SQuAD](https://huggingface.co/datasets/squad)

## Setup Environment

Run the following commands to setup a conda environment:

````
conda create --name embedding_recycling --file requirements.txt
conda activate embedding_recycling
````

## Experiment Replication

# Standard Embedding Recycling

To replicate our results for standard embedding recycling, use the conda environment listed above and run the following scripts for each dataset group:

- For text classification, use the `TextClassificationScripts/GeneralLinearClassifier_PaperResults.py` script
- For NER, use the `NER_Scripts/General_NER_Classifier_PaperResults.py` script
- For QA, use the `QA_Scripts/GeneralQuestionAnswering_PaperResults.py` script to replicate the TriviaQA results. For SQuAD, please use the "run_squad.py" script included on the [HuggingFace Transformers repository](https://github.com/huggingface/transformers/blob/main/examples/legacy/question-answering/run_squad.py), which we also include in our main directory.

The hyperparameters for replicating each experiment are included in the `HyperparameterSelection` folder. 

# Adapter-Based Embedding Recycling

To replicate our results for adapter-based embedding recycling, use the conda environment listed above and run the following scripts for each dataset group:

- For text classification, use the `TextClassificationScripts/Adapters_PaperResults.py` script
- For NER, use the `NER_Scripts/Adapters_NER_PaperResults.py` script
- For QA, use the `QA_Scripts/Adapters_QA_PaperResults.py` script to replicate the TriviaQA results. For SQuAD, please use the "run_squad.py" script included on the [HuggingFace Transformers repository](https://github.com/huggingface/transformers/blob/main/examples/legacy/question-answering/run_squad.py), which we also include in our main directory.

The hyperparameters for replicating each experiment are included in the `HyperparameterSelection` folder. 
