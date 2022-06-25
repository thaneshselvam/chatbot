# Chatbot Deployment with Flask and JavaScript

In this tutorial we deploy the chatbot I created in [this](https://github.com/python-engineer/pytorch-chatbot) tutorial with Flask and JavaScript.

This gives 2 deployment options:
- Deploy within Flask app with jinja2 template
- Serve only the Flask prediction API. The used html and javascript files can be included in any Frontend application (with only a slight modification) and can run completely separate from the Flask App then.

## Initial Setup:
This repo currently contains the starter files.

Clone repo and create a virtual environment
```
git clone https://github.com/python-engineer/chatbot-deployment.git
cd chatbot-deployment
py -m venv venv
venv/Scripts/activate
```
Install dependencies
```
(venv) pip install Flask torch torchvision nltk
```
Install nltk package
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



