<!-- omit in toc -->
# flask-bootstrap4-heroku-skeleton

<!-- omit in toc -->
## Table of Contents
<details>
<summary>Click to expand</summary>

- [1. Introduction](#1-introduction)
- [2. Setup](#2-setup)
	- [2.1. Get virtualenv](#21-get-virtualenv)
	- [2.2. Create a virtual enviroment](#22-create-a-virtual-enviroment)
	- [2.3. Activate enviroment](#23-activate-enviroment)
	- [2.4. Install requried packages](#24-install-requried-packages)
	- [2.5. Run The Application](#25-run-the-application)
	- [2.6. Push to Heroku](#26-push-to-heroku)
- [3. License](#3-license)
- [4. Contributors](#4-contributors)

</details>

## 1. Introduction

This is a template project used to kickstart a Flask project containing:

* Bootstrap 4.5.2 CDN
* Procfile for Heroku
* python-dotenv for setting up local variables

## 2. Setup

Make sure to have Python 3.6 or newer, and pip installed.

### 2.1. Get virtualenv

```console
$ pip install virtualenv
```

### 2.2. Create a virtual enviroment

Make sure to create a Python3 instead of Python2 enviroment by refrencing its binaries.
```console
$ which python3
/usr/bin/python3
```

You can use any name you want, we will use "venv".
```console
$ virtualenv -p /usr/bin/python3  venv
```

### 2.3. Activate enviroment

```console
$ . venv/bin/activate
```

Now you have activated your virual enviroment and your teminal should display its name as so:
```console
$(venv)
```

### 2.4. Install requried packages
```console
$(venv) pip3 install -r requirements.txt  
```

### 2.5. Run The Application

```console
$(venv) flask run
```

You’ll see output similar to this:

```console
Serving Flask app "app"
Environment: development
Debug mode: on
Running on http://127.0.0.1:5000/
Restarting with stat
Debugger is active!
Debugger PIN: 298-204-950
```

Open the link in your browser.

### 2.6. Push to Heroku
Make sure you have installed Heroku CLI, and have authentication to the Heroku project.

Install the [Heroku CLI](https://devcenter.heroku.com/articles/heroku-command-line)
Download and install the Heroku CLI.

If you haven't already, log in to your Heroku account and follow the prompts to create a new SSH public key.
**Login into Heroku**
```console
$ heroku login
```

**Clone the repository**
Use Git to clone heroku-app's source code to your local machine.


```console
$ heroku git:clone -a <heroku-app>
$ cd <heroku-app>
```

**Deploy your changes**
Make some changes to the code you just cloned and deploy them to Heroku using Git.

```console
$ git add .
$ git commit -am "make it better"
$ git push heroku master
```

## 3. License
This project is licensed under the Apache License, Version 2.0 - see the [LICENSE](LICENSE) file for details.

## 4. Contributors
<a href="https://github.com/egillanton/flask-bootstrap4-heroku-skeleton/graphs/contributors">
  <img src="https://contributors-img.web.app/image?repo=egillanton/flask-bootstrap4-heroku-skeleton" />
</a>
<!-- Made with [contributors-img](https://contributors-img.web.app). -->

[Become a contributor](CONTRIBUTING.md)

<p align="center">
🌟 PLEASE STAR THIS REPO IF YOU FOUND SOMETHING INTERESTING 🌟
</p>