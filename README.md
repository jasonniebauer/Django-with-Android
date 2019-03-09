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
Install [Termux](https://termux.com/), launch and update it.

**Update**
```
pkg update && pkg upgrade
```

You can use the [apt command](https://en.wikipedia.org/wiki/APT_(Debian)) if your prefer. 
```
apt update && apt upgrade
```

**Tip**: Enlarge the font size by pressing <kbd>CTRL</kbd>+<kbd>Alt</kbd>+<kbd>+</kbd>

#### Setup External Storage
Create a storage directory to access other areas of the device.
```
termux-setup-storage
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
Change directories to the newly created `storage` folder.
```
cd storage
```

Create a directory to store our project files.
```
mkdir myapp && cd myapp
```

### Virtual Environment
Now that we are in our newly created project folder it's time to setup a [virtual environment](https://docs.python.org/3/tutorial/venv.html) for our app.

#### Create Virtual Environment
```
python -m venv <virtual environment name>
```

Example:
```
python -m venv venv
```

#### Activate Virtual Environmemt
What good is a virtual environment if it's not being used? That's right, we need to activate it to use it.

```
source <venv>/bin/activate
```

Example:
```
source venv/bin/activate
```

**Tip**: Close out of a virtual environment by typing `deactivate` and then hitting <kbd>Enter</kbd>

### Install Django
Our virtual environment is activated and we're ready to install Django.

```
pip install django
```

**Save installed packages to a text file**
```
pip freeze > requirements.txt
```

## Django Setup

### Start Project
Tell Django admin to start a new project with your project name.

```
django-admin startproject <project name>
```

Example:
```
django-admin startproject myapp
```

Change into the Django project directory to view the files Django generated
```
cd <project name>
```

Example:
```
cd myapp
```

### Start App
Tell Django to run a local server and watch for changes
```
python manage.py runserver
```

Open your web browser and navigate to `localhost:8000` to confirm the Django app is running successfully!

**Tip**: Stop the local server from running by hitting <kbd>CTRL</kbd>+<kbd>c</kbd>
