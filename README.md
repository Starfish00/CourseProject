# CourseProject

Please fork this repository and paste the github link of your fork on Microsoft CMT. Detailed instructions are on Coursera under Week 1: Course Project Overview/Week 9 Activities.

# App instructions

## Online Webapp

https://cs410-proj.onrender.com/ And just input a sentence to get its sarcastic probability

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

Finally, you may want to deactivate the virtual environment
```
deactivate
```
