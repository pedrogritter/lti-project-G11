# lti-project-G11
Django application for scheduling, monitoring and grading classes. 

#### Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

#### Prerequisites
What things you need to install the software and how to install:
1. Python 3
2. Django 2.1.7


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
sudo yum install python3-devel # Red Hat / CentOS

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

[Django Packages](https://djangopackages.org/)- A directory of reusable apps, sites, tools, and more for your Django projects.


## Useful Docs
[Full Stack Python](https://www.fullstackpython.com/table-of-contents.html) - A collection of everything web related to Python.

[Django 2.x Basic Commands](https://gist.github.com/bradtraversy/0df61e9b306db3d61eb24793b6b7132d)

[Vue.js Cheatsheet](https://vuejs-tips.github.io/cheatsheet/) - Vue.js 2.2 complete API cheatsheet 

[Bulma Basic Elements](http://yingyingzhang.com/bulma-cheat-sheet/assets/bulma-cheat-sheet-7-2-2018.pdf) - Most available Bulma classes and modifiers.

## Recommended Tutorials
[Django 1h Crash Course](https://www.youtube.com/watch?v=D6esTdOLXh4&t=1461s) - The framework and its advantages, setup up an app from scratch with MySQL. The MTV (Model-Template-View) design pattern, setup a virtual environment, look at the core Django files and build the app.

[Vue.js 2.0 in 60 Minutes](https://www.youtube.com/watch?v=z6hQqgvGI4Y&t=106s) - Covers all of the fundamentals of the Vue.js 2.0 JavaScript framework. 

[Bulma CSS Framework Crash Course](https://www.youtube.com/watch?v=IiPQYQT2-wg) - A crash course and resource guide with most of the elements that are available including the navigation, typography, boxes, grid system, forms, tables , etc.

[Simple CRUD App with Django & Vue.js](https://medium.com/quick-code/crud-app-using-vue-js-and-django-516edf4e4217) - How to make a simple CRUD application using Vue.js 2.x and Django 2.0.2. Vue.js is used for building user interfaces and Django, a high level python Development framework that encourages rapid Develpoment.

