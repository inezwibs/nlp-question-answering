# nlp-question-answering
## Summary
The purpose of this package is to provide learning modules for building Question Answering systems
utilizing combination of NLP techniques and Knowledge Graphs.

## Installation
This package can be used in 2 ways: using docker or directly using python3.

### Using Python3
1. Ensure that you have python3 installed on your system.
2. Install prerequisites: ```sudo apt-get install libmysqlclient-dev```
3. Install following python packages: ```pip3 install word2number gitpython progressbar colorama pattern google-api-python-client requests_cache```
4. Install nltk: ```pip3 install --user -U nltk```
5. Download ntlk's stopwords and punkt data packages: see https://www.nltk.org/data.html.
6. Get this git repository
7. Run setup script: ```python3 setup_env.py```

### Using docker 
1. Ensure you have docker installed on your system
2. Download Dockerfile from this repository
3. Build docker image by running: "docker build -t nlp-question-answering ."
4. Run docker container by running: "docker run -it nlp-question-answering"

## Usage
The package allows users to run individual parts of sample Question Answering pipeline. 
The module to run is specified via the parameter, as well as the question to be processed.
For example, to run QPM module, the following command can be used:
```
>python3 module_run.py --module=qpm --question="How tall is Mount McKinley?"
```
For a list of available modules, run:
```
>python3 module_run.py --help
```
