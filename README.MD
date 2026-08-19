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
django-tutorials/
│
├── 01-basics/              # Introduction to Django, views, URLs, and templates
├── 02-models-and-orm/      # Database migrations, models, and Django ORM queries
├── 03-forms-and-admin/     # Working with Django forms, ModelForms, and the admin panel
├── 04-class-based-views/   # Implementing CBVs (ListView, DetailView, CreateView, etc.)
└── 05-rest-framework/      # Building APIs using Django REST Framework (DRF)

```


#  Getting Started Locally

To run any of the tutorial modules or mini-projects on your local machine, follow these steps:

# 1. Clone the repository

```bash
git clone https://github.com/zuck30/django_tutorials.git
cd django_tutorials

```

#  2. Create and activate a virtual environment

```bash
python -m venv --without-pip thisdjango
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source thisdjango/bin/activate

```

# 3. Install dependencies

```bash
pip install -r requirements.txt

```

# 4. Run migrations

Navigate into a specific project folder containing `manage.py`, then run:

```bash
python manage.py migrate

```

# 5. Start the development server

```bash
python manage.py runserver

```

# Learning Objectives

* Understand the MVT (Model-View-Template) architectural pattern.
* Master database design and efficient querying using the Django ORM.
* Implement secure user authentication and authorization workflows.
* Build scalable RESTful APIs with Django REST Framework.


# Contributing

Feel free to fork this repository, open issues, or submit pull requests if you have suggestions, optimizations, or alternative approaches to the exercises!