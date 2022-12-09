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

Install required packages

```
pip install -r requirements.txt
```

If some particular package is still missing, do something like

```
pip install scikit-learn
```

Running the program
```
python app.py
```

If you're on Mac and have Python3, you might want to run
```
python3 app.py
```

If the last command doesn't work

Then the terminal will likely show something like
```
Dash is running on http://127.0.0.1:8050/
```
If port 8050 is already in use, it might give you something else

Paste http://127.0.0.1:8050/ or whatever your terminal is giving you to the browser




