# 🐍 Django Project Setup Guide

This guide explains step-by-step how to create and run a new Django project inside a virtual environment.

---

## 📁 Step 1: Open Terminal and Navigate to Project Folder

cd django_test

## 📦 Step 2: Check Installed Packages (Optional)

pip freeze

## 🌐 Step 3: Create Virtual Environment

python -m venv env

💡 On some systems use python3 instead of python.

## ⚙️ Step 4: Activate Virtual Environment

▶ Windows (PowerShell / CMD)

env\Scripts\activate

▶ macOS / Linux

source env/bin/activate

Once activated, you’ll see (env) before your terminal prompt.

## 🧾 Step 5: Verify Installed Packages

pip freeze

📥 Step 6: Install Django

▶ Specific Version

pip install django==4.1

▶ Latest Version

pip install django

Check installed packages:

pip freeze
Example output:

asgiref==3.8.1
Django==5.2.8
sqlparse==0.5.3

## 🏗️ Step 7: Create a New Django Project

To create a new Django project, use the following command:

django-admin startproject projectname

If you want to create it in the current directory, add a dot . at the end:


django-admin startproject learning .

Your folder structure will look like:


learning/

    __init__.py

    asgi.py

    settings.py

    urls.py

    wsgi.py

db.sqlite3

manage.py

## ▶ Step 8: Run the Development Server

python manage.py runserver

Now open your browser and visit:

👉 http://127.0.0.1:8000

## 📴 Step 9: Deactivate Virtual Environment

deactivate

✅ Project successfully set up!

You can now start building Django apps using:

python manage.py startapp appname

## 📚 Notes

Always activate your environment before installing packages or running the project.

To list all dependencies later, use:

pip freeze > requirements.txt

To install dependencies from the file:

pip install -r requirements.txt

## Author: Suraj Pawar
## Tech Stack: Python · Django · SQLite


