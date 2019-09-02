# nlp_pt-BR_course
NLP for Brazilian Portuguese. For this course we will learn NLP techniques using NLTK, scikit-learn and spaCy.


## Installing project dependencies

You must have installed Python 3.5+ and `pip`.

First of all, we need to install `virtualenv`. Basically, virtualenv is a tool to create isolated Python environments.

```
$ pip install virtualenv
```

Create a `virtualenv` dir to install all the project dependencies.

```
$ virtualenv -p python3 venvvirtual venv  
```

Then, activate the environment. You'll see a `(venv)` at the beginning of the promp:

```
$ source venv/bin/activate
```

Install all python dependencies:

```
(venv) $ pip install -r requeriments
```

To work with Portuguese language using spaCy, we need to install the multi-task model trained on the Universal Dependencies and WikiNER corpus. This model has POS tags, dependency parse and named entities. Supports identification of PER, LOC, ORG and MISC entities.

```
(venv) $ python -m spacy download pt_core_news_sm
```

That's all! See the wiki to see the NLP course using NLTK and spaCy.
