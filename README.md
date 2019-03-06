# Django for Android

**Table of Contents**
1. [Get Started](#get-started)  
    1.1 [Install Termux](#install-termux)  
    1.2 [Install Python](#install-python)  
    1.3 [Install Git](#install-git)  
2. [Project Setup](#project-setup)  
    2.1 [Local Directory](#local-directory)  
    2.2 [Virtual Environment](#virtual-environment)  
    2.3 [Install Django](#install-django)  
3. [Django Setup](#django-setup)  
    3.1 [Start Project](#start-project)  
    3.2 [Start App](#start-app)  

## Get Started 
### Install Termux
Install [Termux](https://termux.com/) for Android.

**Upgrade**
```
pkg upgrade
```

### Install Python
**Install Python**
```
pkg install python
```

### Install Git
**Install Git**
```
pkg install git
```

## Project Setup

### Local Directory
Create a directory to store our project files.
```
mkdir myapp
```

Change directories to the newly created project folder.
```
cd myapp
```

### Virtual Environment

#### Create Virtual Environment
```
python -m venv <virtual environment name>
```

Example:
```
python -m venv venv
```

#### Activate Virtual Environmemt

```
source <venv>/bin/activate
```

Example:
```
source venv/bin/activate
```

### Install Django

```
pip install django
```

```
pip freeze > requirements.txt
```

## Django Setup

### Start Project
```
django-admin startproject <project name>
```

Example:
```
django-admin startproject myapp
```

## Run Django

```
cd <project name>
```

Example:
```
cd myapp
```

```
python manage.py runserver
```

Open your web browser and navigate to `localhost:8000` to confirm the Django app is running successfully.

Stop the local server from running by hitting <kbd>CTRL</kbd>+<kbd>c</kbd>
