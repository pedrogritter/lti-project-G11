# Sigma
Django application for scheduling, monitoring and grading classes. 

#### Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

#### Prerequisites
What things you need to install the software and how to install:
1. Python 3
2. Django 2.1.7
3. PostgreSQL

#### Install PostgreSQL - In case it is not installed in the system

+ Start by updating the apt-get’s list of packages:

```
sudo apt-get update
```

+ Next, install Postgres by entering the following command in the terminal:

```
sudo apt-get install postgresql postgresql-contrib libpq-dev
```

+ By default Postgres creates a postgres user and is the only user who can connect to the server. We’ll want to create ourselves on the server with superuser capabilities with the same name as our login name:

```
sudo -u postgres createuser --superuser $USER
```

+ Enter your desired password when prompted.

+ Next, we’ll have to create a database with the same name as our login name since this is what Postgres expects by default when connecting to the server with your login name:

```
sudo -u postgres createdb $USER
```

+ Navigate to your home directory and enter the following command to create the .psql_history in order to save your history:

```
touch .psql_history
```
+ Type psql on your terminal to connect to the server:

```
psql (10.6 (Ubuntu 10.6-0ubuntu0.18.04.1))
Type "help" for help.

user=# 
```

+ Enter \q to quit and return to your terminal.



#### Installing 
Here is a step by step series of examples that tell you how to get a development env running

+  Create or go to the desired folder destination

+  Create a virtual environment:

```
virtualenv venv
```

+  **__In case you use Python 2.7__**

   Change the version of Python for the virtual environemnt with this command:
   
```
virtualenv --python=/usr/bin/python3.6 venv
```

+ Activate the environment:

```
. venv/bin/activate
```

If it worked, terminal prompt should be similar to this:

```
(venv) User@computer-UX430UAR:~/Documents/lti-project-G11$
```

+  Clone the repository to the destination folder

```git
git clone https://github.com/pedrogritter/lti-project-G11.git
```
+ Install required dependencies by running:

```
Note on Python 3 :you need to install python3-dev using the following command :
sudo apt-get install python3-dev # debian / Ubuntu

And the python3 mysql library: 

sudo apt-get install python3.6-dev libmysqlclient-dev
```
```
pip install Django==2.1.7
pip install mysqlclient
```

#### Deployment
~~This project is deployed on [Heroku](https://www.heroku.com/) over [here](https://lti-project-G11.herokuapp.com/)~~

To deploy this on a live system enter the following command:

```
python manage.py runserver
```
A development server should be running at http://127.0.0.1:8000/


## Built With

[Django 2.1.7](https://www.djangoproject.com/)- Python Web framework used

[Vue.js 2.2](https://vuejs.org/) - Progressive Javascript framework

[Bulma](https://bulma.io)- Modern CSS Framework

[PostgreSQL](https://www.postgresql.org/)

[Django Packages](https://djangopackages.org/)- A directory of reusable apps, sites, tools, and more for your Django projects.
