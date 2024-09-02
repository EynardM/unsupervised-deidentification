
Note: All commands in this document should be executed from the root directory

# Working Environment

To install all required packages for running the files, execute the following command:

**pip install -r requirements.txt**

# Datasets

## Training datasets
To obtain the training datasets, execute: **datamodule.py**
Training datasets can be visualized in the folder: **Datasets/Training_Datasets**

## Deididentified datasets
To obtain the deidentified datasets, execute: **deid.py**
Deididentified datasets can be visualized in the folder: **Datasets/Deid_Datasets**
METHODS : *IDF, IDF-table-aware, Lexical, Ner*

# Training Reidentification Models
First Approach (**finetuning.py**)
This method is based on the paper: *Unsupervised Text Deidentification John X. Morris Justin T. Chiu Ramin Zabih Alexander M. Rush*.
However, no satisfactory results were achieved. The attempted model for reidentification in this script is *Roberta-Roberta*.

Second Approach (**model.py**)
We directly trained our networks using a script similar to model.py. 
Note: GPUs were used for running this type of script. Sometimes, you may need to adapt the input of your model, as it can take tokens or embeddings.

# Results
To obtain the results, run: **python result.py**
Note: The last model is not yet functional in this file.

# Appendices
Imports: **imports.py**
Functions: **functions.py**
Paths: **locations.py**
Parameters: **parameters.py**

