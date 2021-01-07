# [Flask](https://palletsprojects.com/p/flask/) Tutorial

> Content provided by experienced developers based on the suggestions/questions from the audience. This initiative aims to provide **Free/Allways up-to-date** programming tutorials - Read the [Manifest](https://github.com/app-generator/learn-to-code).

<br />

**How it works**

- Access the existing content
- Open a [new issue](https://github.com/app-generator/tutorial-flask/issues/new) to get an answer related to an existing topic
- Open a [new issue](https://github.com/app-generator/tutorial-flask/issues/new) to open a new tutorial topic
- Answers will be provided by experienced contributors 
- Vote the response

<br />

**Become a contributor**  

- Open a [new issue](https://github.com/app-generator/tutorial-flask/issues/new) using **Contributor** word in the title. Please provide relevant information regarding your experience. 

<br />

## Topics

- [What is Flask](#what-is-flask)
- [How can I install Flask](#how-can-i-install-flask)
- [A minimal Flask application](#a-minimal-app)
- [Flask Project Structure](#flask-project-structure)

<br />

## What is Flask

:point_right: Flask is a lightweight web application framework. It is designed to make getting started quick and easy, with the ability to scale up to complex applications.
Compared to [Django](https://www.djangoproject.com/), Flask provides a lightweight codebase and more freedom to the developer.

<br />

> [Go UP :point_up_2:](#topics) 

<br />

## How can I install Flask

:point_right: The easiest way to install [Flask](https://palletsprojects.com/p/flask/) is to use [PIP](https://pip.pypa.io/en/stable/quickstart/) the official package-management tool.

```bash
$ pip install Flask
```

<br />

**How to check Flask version**

Open a Python console (type python in terminal) and check the installed version as below:

```python
>> import flask
>> flask.__version__
'1.1.2' 
>>>
```

In this case the installed version is **1.1.2**

<br />

<p align="right"><a href="#topics"> :up: Return to top</a></p>

<br />

## A minimal App

:point_right: Open a terminal and install Flask (if not already installed) using PIP:

```bash
$ pip install Flask
```

Use your preferred editor to create a file called **hello.py** with this content:

```python
from flask import Flask

app = Flask(__name__)

@app.route('/')
def hello():
    return f'My first Flask!'
```

Save the file and start the app:

<br />

```bash
$ env FLASK_APP=hello.py flask run
 * Serving Flask app "hello"
 * Running on http://127.0.0.1:5000/
```

Above commnand does two things:

- Set the `FLASK_APP` variable (required by Flask)
- Execute our code with `flask run` command

<br />

By visiting the app in the browser **localhost:5000** we should see **My first Flask!** message.

<br />

> [Go UP :point_up_2:](#topics) 

<br />

## [Flask Project Structure](./flask-project-structure.md)

:point_right: Being such a lightweight framework, Flask comes with great flexibility regarding the codebase structure of a project. We can use a single file and drop all the code or split the app logic in more files and directories. All variants works but we migth have issues once our project is getting bigger and migth become unreadable for others. 

Well, this section presents a few options to keep in mind when we start a Flask project. 


> Read in detail: [Flask Project Structure](./flask-project-structure.md) 

<br />

> [Go UP :point_up_2:](#topics) 

<br />

---
**[Flask](https://palletsprojects.com/p/flask/) Tutorial** - Free/Allways up-to-date Flask-related content | by [AppSeed](https://appseed.us?ref=gh).
