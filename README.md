Image CLassification:

This repo contain thre categories. 

<B> Setting up the Environment</B>
```
python3 -m pip install -U virtualenv # install the virtualenv
virtualenv -p python3 dev_env # creating an environment
source dev_env/bin/activate # activate environment
git clone https://github.com/entiretydotai/Image-Classification-and-Deployment #clone the repo
cd Image-Classification-and-Deployment
pip install -r requirements.txt # install the requirements
```

Deep learning model: For classification, transfer learning techniques has been used as it has preweights. I also some of the layer on top of that. 
Once it has been trained, I have save model so we can directly use on other dataset. 

Now we have to make API so we can predict label according to that. we will use flask for creating web app. 
let's take an example of flask:
from flask import Flask
'''
app = Flask(__name__)

@app.route("/")
def hello_world():
    return "<p>Hello, World!</p>"

'''

In gui of webapp, user can upload image as a output they got to know that image is from which category. 

<B> UPLOAD IMAGES</B>

![upload image](https://github.com/Milanbhadja/classification/blob/main/static/upload_image.png)

<b> Prediction</b>

![predicted result](https://github.com/Milanbhadja/classification/blob/main/static/prediction%20image.png)

Craete new virtual enviornment to install all dependencies. 

After that all app has been dockerised with docker. 

Once it has been contenerised, create CI/CD pipeline for github action.



