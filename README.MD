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

*(Note: Running `migrate` translates Django's built-in blueprint files into actual tables inside your SQLite database for user authentication, admin logs, and sessions.)*

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

# Learning Objectives

* Understand the MVT (Model-View-Template) architectural pattern.
* Master database design and efficient querying using the Django ORM.
* Implement secure user authentication and authorization workflows.
* Build scalable RESTful APIs with Django REST Framework.

# Contributing

Feel free to fork this repository, open issues, or submit pull requests if you have suggestions, optimizations, or alternative approaches to the exercises!