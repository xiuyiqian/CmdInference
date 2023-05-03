**Command Inference**
==========================

Introduction
------------

`Command Inference` serves for READY PLAYER EVE text/speech trigger animation.
Purpose: when the user gives the command, the user will be given further question regarding to the command for guidance. 

Documentation
-------------

[Spacy Documentation](https://spacy.io/usage/linguistic-features).



Installation
------------

### Conda virtual environment

recommend setting up a fresh Conda environment to run the jupyter notebook.

```bash
conda create --name cmdInfer python==3.8
conda activate cmdInfer
```

###  Pip

Use this installation mode if you want the latest released version.
```
pip install spacy
pip install nltk
spacy.cli.download("en_core_web_sm")
nltk.download(['stopwords','punkt',"names","stopwords","state_union","twitter_samples","movie_reviews","averaged_perceptron_tagger","vader_lexicon","punkt"])
```

**_NOTE:_** "en_core_web_sm" is a medium sized English model trained on written web text (blogs, news and comments) including a word vector table with 2


### Animation Dictionary

Each object/noun has corresponding verbs acting on it.
Each verb/action has corresponding questions if necessary.

### Process Explaination/Result
| Function Name      | Description | Result |
| ----------- | ----------- | ----------- |
| nvn     | Quick-start guide       |
|    |         |


 
### Improvement

* Currently, the question only will be asked if the command's extracted verb matches exactly same as the key in the json library. We could compute the similiarity between the key of the dictinoary and the command's action word to allow flexibility. 
