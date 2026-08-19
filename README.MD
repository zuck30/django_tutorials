# Django Tutorials

Welcome to my Django learning repository! This project serves as a structured workspace where I am building, testing, and documenting my progress as I master backend web development with Django.

# Tech Stack & Tools

* **Language:** Python
* **Framework:** Django
* **Database:** SQLite (default for development) / PostgreSQL (for production-ready practice)
* **Version Control:** Git & GitHub

# Repository Structure

The repository is organized by topics and mini-projects as I progress through the learning curriculum:

```text
django_tutorials/
├── thisdjango/             # Python virtual environment
├── zuck_django_tutorials/  # Main Django project container
│   ├── 01-basics/          # Introduction to Django, views, URLs, and templates
│   ├── 02-models-and-orm/  # Database migrations, models, and Django ORM queries
│   ├── 03-forms-and-admin/ # Working with Django forms, ModelForms, and the admin panel
│   ├── 04-class-based-views/# Implementing CBVs (ListView, DetailView, CreateView, etc.)
│   └── 05-rest-framework/  # Building APIs using Django REST Framework (DRF)


```

# Getting Started Locally

To run any of the tutorial modules or mini-projects on your local machine, follow these steps:

# 1. Clone the repository

```bash
git clone https://github.com/zuck30/django_tutorials.git
cd django_tutorials


```

# 2. Create and activate a virtual environment

```bash
python -m venv thisdjango
# On macOS/Linux:
source thisdjango/bin/activate
# On Windows:
thisdjango\Scripts\activate


```

# 3. Install dependencies / Django

```bash
pip install --upgrade pip
pip install django
# Or if a requirements file exists:
# pip install -r requirements.txt


```

# 4. Create your Django project (if starting fresh)

```bash
django-admin startproject zuck_django_tutorials


```

# 5. Run migrations

Navigate into your project folder containing `manage.py`, then run:

```bash
cd zuck_django_tutorials
python manage.py migrate


```
>[!IMPORTANT]
>*(Note: Running `migrate` translates Django's built-in blueprint files into actual tables inside your SQLite database for user authentication, admin logs, and sessions.)*

# 6. Start the development server

```bash
python manage.py runserver


```

# Create App

> [!IMPORTANT]
>I will Start by navigating to the selected location where I want to store the app, in my case the zuck_django_tutorials folder, and run the command below. If the server is still running, and you are not able to write commands, press [CTRL] [BREAK], or [CTRL] [C] to stop the server and you should be back in the virtual environment. I will name my app members.

```bash
python manage.py startapp members
```

# Django Views

>Django views are Python functions that take http requests and return http response, like HTML documents. A web page that uses Django is full of views with different tasks and missions. Views are usually put in a file called views.py located on our app's folder (members folder). There is a views.py in our members folder. Please Find it.


>[!IMPORTANT]
>Note that: The name of the view does not have to be the same as the application. I call it members because I think it fits well in this context.

# Django URLs

Create a file named urls.py in the same folder as the views.py file. Already did that, see the code in the file

>The urls.py file that we just created is specific for the members application. We have to do some routing in the root directory zuck_django_tutorials as well. This may seem complicated, but for now, just follow the instructions below.
# Pay attention

>[!IMPORTANT]
>There is a file called urls.py on the zuck_django_tutorials folder, open that file and add the include module in the import statement, and also add a path() function in the urlpatterns[] list, with arguments that will route users that comes in via 127.0.0.1:8000/.

# About Urls
Think of it like giving someone directions to your house:

1. **Main URL (`zuck_django_tutorials/urls.py`):** You tell your friend, *"Go to **Street: Members**."*
2. **App URL (`members/urls.py`):** Inside that street, you told them, *"Now walk down **Street: Members** again to find the house."*

Because there isn't a second "Members" street, they get lost and hit a wall.

By changing the app URL to an empty string (`''`), you are saying: *"Once you arrive at **Street: Members**, stop right here—this is the house."*

# Learning Objectives

* Understand the MVT (Model-View-Template) architectural pattern.
* Master database design and efficient querying using the Django ORM.
* Implement secure user authentication and authorization workflows.
* Build scalable RESTful APIs with Django REST Framework.

# Contributing

Feel free to fork this repository, open issues, or submit pull requests if you have suggestions, optimizations, or alternative approaches to the exercises!