# nlp_pt-BR_course
NLP for Brazilian Portuguese. In this course we will learn useful NLP techniques using NLTK, scikit-learn and spaCy.


## Installing project dependencies

You must have installed `Python 3.6+` and `pip`.

First of all, we need to install `virtualenv`. Basically, `virtualenv` is a tool to create isolated Python environments.

```
$ pip install virtualenv
```

Create a `virtualenv` environment to install all the project dependencies.

```
$ virtualenv -p python3 venv  
```

Then, activate the environment. You'll see a `(venv)` at the beginning of the promp:

```
$ source venv/bin/activate
```

Install all the Python dependencies:

```
(venv) $ pip install -r requirements.txt
```

Install NLTK packages

```
python -m nltk.downloader stopwords
python -m nltk.downloader rslp
python -m nltk.downloader punkt
python -m nltk.downloader machado
python -m nltk.downloader mac_morpho
```

To work with Portuguese language using spaCy, we need to install the multi-task model called `pt_core_news_sm`. This model was trained on the Universal Dependencies and WikiNER corpus. The model has POS tags, dependency parse and named entities. Supports identification of PER, LOC, ORG and MISC entities.

```
(venv) $ python -m spacy download pt_core_news_sm
```

Open *Jupyter Notebook* using following command:

```
(venv) $ jupyter notebook
```

If Jupyter doesn't **recognize** your environment, please run the following command:

```
(venv) $ python -m ipykernel install --user --name=venv
```

That's all! You will find the courses (NLTK and spaCy) inside `notebooks` dir and the presentation in `docs` dir.

