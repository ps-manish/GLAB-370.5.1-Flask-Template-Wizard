# GLAB-370.5.1-Flask-Template-Wizard

## Welcome to the "Flask Template Wizard: Creating and Using Templates in Flask" Guided Lab! 🚀

In this 30-minute guided lab, we'll embark on an exciting coding adventure that focuses on **creating and using templates** in Flask. Get ready to unleash the power of templates to build dynamic and interactive web pages!

### Prerequisites

Before we begin, make sure you have the following:

- Flask installed (if not, run `pip install flask` in your terminal).
- Basic knowledge of Python syntax.
- A Python interpreter or an integrated development environment (IDE) installed on your machine.

### Table of Contents

- [Step 1: Introduction](#step-1-introduction)
- [Step 2: Creating a Templates Directory](#step-2-creating-a-templates-directory)
- [Step 3: Defining a Basic HTML Template](#step-3-defining-a-basic-html-template)
- [Step 4: Using Templates in Flask](#step-4-using-templates-in-flask)
- [Step 5: Challenge](#step-5-challenge)
- [Step 6: Conclusion](#step-6-conclusion)

### Step 1: Introduction

Let's begin our adventure into the world of Flask templates. Templates are a powerful tool that allow us to separate the presentation logic from the application logic in Flask. In this lab, we'll learn how to create templates and use them in our Flask application.

### Step 2: Creating a Templates Directory

To start, create a directory named `templates` in your Flask application's root directory. This is where we'll store our HTML templates. Flask automatically looks for templates in this directory.

### Step 3: Defining a Basic HTML Template

Create an HTML file inside the `templates` directory, e.g., `index.html`. This will be our basic template. You can use any text editor or an HTML editor of your choice.

In `index.html`, add the following HTML code:

```html
<!DOCTYPE html>
<html>
<head>
    <title>My Flask App</title>
</head>
<body>
    <h1>Welcome to my Flask App!</h1>
    <p>This is a basic Flask template.</p>
</body>
</html>
```

This is a simple HTML template that displays a heading and a paragraph. We'll use this template in our Flask application.

### Step 4: Using Templates in Flask

Now, let's create a Flask application that uses the template we just created.

Create a Python file, e.g., `app.py`, and add the following code:

```python
from flask import Flask, render_template

app = Flask(__name__)

@app.route("/")
def home():
    return render_template("index.html")

if __name__ == "__main__":
    app.run()
```

In this code, we import the `render_template` function from Flask, define a route `/` with a corresponding view function `home()` that uses the `render_template` function to render the `index.html` template.

### Step 5: Challenge

Now it's time for an exciting challenge! Customize your template by adding more HTML elements, styling with CSS, or introducing dynamic content using template variables. Experiment with different Flask features, such as passing data to templates, conditionals, or loops. Make your Flask application shine with your creativity!

### Step 6: Conclusion

Congratulations on completing the "Flask Template Wizard: Creating and Using Templates in Flask" Guided Lab! You've successfully created and used templates in Flask, separating the presentation logic from the application logic.

Remember to keep exploring Flask's template capabilities and experiment with different features and functionalities. Flask templates provide a flexible and powerful way to create dynamic and

 interactive web pages.

Feel free to reach out if you have any questions. Happy coding, and may your Flask templates bring life to your web applications! 🎉
