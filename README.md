# Chatbot Deployment with Flask and JavaScript

## Initial Setup:
This repo currently contains the starter files.

Clone repo and create a virtual environment
```
git clone https://github.com/python-engineer/chatbot-deployment.git
cd chatbot-deployment
py -m venv venv
venv\Scripts\activate
```
Install dependencies
Flask is for web creation
nltk is natural languange toolkit
```
(venv) pip install Flask torch torchvision nltk
```
Install nltk package
Natural language
```
(venv) py
>>> import nltk
>>> nltk.download('punkt')
```
Modify `intents.json` with different intents and responses for your Chatbot. Everytime intends are updated it must be trained again.

Run
```
(venv) py train.py
```
This will dump data.pth file. And then run
the following command to test it in the console.
```
(venv) py chat.py
```



