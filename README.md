# CourseProject

Please fork this repository and paste the github link of your fork on Microsoft CMT. Detailed instructions are on Coursera under Week 1: Course Project Overview/Week 9 Activities.

# Function
<ul>
  <li>Webbapp: The webapp can be used to identify how sarcastic an input sentence is. After opening up the website, there is an input box where the user can input a sentence. The user just simply need to click the 'Submit' button once a sentence is typed and a 'sarcastic probability' will be shown under the button.</li>
  <li>Jupter Notebook: The Jupter Notebook should be more regarded as a visualization of the development process. It contains some visualization of the dataset and also clues of how a large back-end language model can improve the identification performance of the webapp.</li>
 </ul>

# Contributions
<ul>
  <li>Anqi & Majharul: Data preprocessing, generating graphs</li>
  <li>Hang: Train a Bert-based model with Pytorch in Jupyter Notebook</li>
  <li>Tianhao: Webapp developed in Dash with packages such as scikit-learn, deployed to render.com</li>
 </ul>


# Jupter Notebook instruction


Assume you're already in the CourseProject folder, having done the following

CD into a directory that you want to work on

On terminal
```
git clone git@github.com:Starfish00/CourseProject.git
```

Go to the CourseProject folder

```
cd CourseProject
```

Then, if you have Anaconda installed. You can simply do this in terminal

```
jupyter notebook
```

Then you will see the notebook on your brower

Finally, if you're on a virtual environment, you may want to deactivate the virtual environment
```
deactivate
```

# Webapp instructions



## Online Webapp

https://cs410-proj.onrender.com/ 

The usage is extremely straightforward, put in a sentence and it will return a probability such that it is sarcastic.

## Introduction

<ol>
  <li>Data preprocessing by getting rid of HTML tags, stemming, converting to lower case, stemming, getting rid of stopwords etc.</li>
  <li>Extract words and bi-grams from sentence</li>
  <li>Used tfidf to build features for model training</li>
  <li>Applied a logistic regression to serve the model, for demonstration purposes. Ran into a whole series of problems when deploying the app to the web due to the environment/dependencies/servers not having the most updated package available. Hang using a Bert-related model in the Jupyter Notebook, which is a way more fancier model than the one in the App. </li>
</ol>

## Testing on your own computer

CD into a directory that you want to work on

On terminal
```
git clone git@github.com:Starfish00/CourseProject.git
```

Go to the CourseProject folder

```
cd CourseProject
```

If you want to create a virtual environment (I strongly suggest you doing so, since you might be running other students' code as well), follow instructions in https://docs.python.org/3/tutorial/venv.html

You can do something like this to create the virtual environment
```
python3 -m venv cs410math-env
```

Do this to activate the environment if you're on Windows
```
cs410math-env\Scripts\activate.bat
```

Do this to activate if you're on Mac
```
source cs410math-env/bin/activate
```

If you still see (base) environment active, do
```
conda deactivate
```

Install required packages

```
pip install -r requirements.txt
```

If some particular package is still missing, do something like

```
pip install scikit-learn
```

Running the program, you might wait for 2 minutes or so for the data preprocessing and model training to run
```
python app.py
```

If you're on Mac and have Python3, you might want to run
```
python3 app.py
```

After a few minutes, the terminal will likely show something like
```
Dash is running on http://127.0.0.1:8050/
```
If port 8050 is already in use (if you're openning another students' app etc.), it might not let you start the program.

Paste http://127.0.0.1:8050/ to the browser

Finally, you may want to deactivate the virtual environment
```
deactivate
```


# Discussion

## Model performance

Both precision, recall and F1 score are above 0.90 for the deep learning model. For details see Jupyter Notebook.

## Limitations of work

We just trained on the title itself, did not utilize the article link. Sometimes whether a title is sarcastic or not will be based on context (such as the article content). This could be a future work item. With that being said, we're satisfied with our current model performance.
