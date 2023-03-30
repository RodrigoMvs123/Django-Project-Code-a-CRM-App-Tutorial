# Django-Project-Code-a-CRM-App-Tutorial

https://www.youtube.com/watch?v=t10QcFx7d5k
https://github.com/flatplanet/Django-CRM.git

https://raw.githubusercontent.com/RodrigoMvs123/Django-Project-Code-a-CRM-App-Tutorial/main/README.md
https://github.com/RodrigoMvs123/Django-Project-Code-a-CRM-App-Tutorial/blame/main/README.md


Django CRM 
Matheus@DESKTOP-3OTOCA6 MINGW64~
$ pwd
/c/Users/Matheus
Matheus@DESKTOP-3OTOCA6 MINGW64~
$ clear
Matheus@DESKTOP-3OTOCA6 MINGW64 ~
$ mkdir  /c/dcrm
Matheus@DESKTOP-3OTOCA6 MINGW64 ~
$ cd  /c/dcrm
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm
$ ls
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm
$ clear
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm
$ python -m venv virt
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm
$ ls
virt/
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm
$ source virt/Scripts/activate
(virt)
$  source virt/Scripts/activate
(virt)
$  source virt/Scripts/activate
(virt)
$  source virt/Scripts/activate
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm
$ clear
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm
$ pip install django 
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm
$ pip install mysql
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm
$ pip install mysql-connector-python
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm
$ clear
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm
$ 
MySQL Community Downloads
https://dev.mysql.com/downloads/file/?id=516466

Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm
$ ls
virt/
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm
$ clear
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm
$ django-admin startproject dcrm
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm
$ ls
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm
$ dcrm/ virt/
(virt) 
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm
$ ls
dcrm/   manage.py*
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm
$ python manage.py startapp website 
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm
$ ls
dcrm/    manage.py    website/
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm
$ 

Django Project – Code a CRM App Tutorial
Django-CRM
dcrm
settings.py

from pathlib import Path

# Build paths inside the project like this: BASE_DIR / 'subdir'.

BASE_DIR = Path(__file__).resolve().parent.parent

# Quick-start development settings - unsuitable for production

# See https://docs.djangoproject.com/en/4.1/howto/deployment/checklist/

# SECURITY WARNING: keep the secret key used in production secret!

SECRET_KEY = 'django-insecure-jcxge@8cwms-4-$&qia^6p+^8-qwrsw7vey#0e6e326apg3mvo'

# SECURITY WARNING: don't run with debug turned on in production!

DEBUG = True
ALLOWED_HOSTS = []

# Application definition

INSTALLED_APPS = [

   'django.contrib.admin',

   'django.contrib.auth',

   'django.contrib.contenttypes',

   'django.contrib.sessions',

   'django.contrib.messages',

   'django.contrib.staticfiles',

   'website',

]

MIDDLEWARE = [

   'django.middleware.security.SecurityMiddleware',

   'django.contrib.sessions.middleware.SessionMiddleware',

   'django.middleware.common.CommonMiddleware',

   'django.middleware.csrf.CsrfViewMiddleware',

   'django.contrib.auth.middleware.AuthenticationMiddleware',

   'django.contrib.messages.middleware.MessageMiddleware',

   'django.middleware.clickjacking.XFrameOptionsMiddleware',

]

ROOT_URLCONF = 'dcrm.urls'

TEMPLATES = [

   {

       'BACKEND': 'django.template.backends.django.DjangoTemplates',

       'DIRS': [],

       'APP_DIRS': True,

       'OPTIONS': {

           'context_processors': [

              'django.template.context_processors.debug',

               'django.template.context_processors.request',

               'django.contrib.auth.context_processors.auth',

               'django.contrib.messages.context_processors.messages',

           ],

       },

   },

]

WSGI_APPLICATION = 'dcrm.wsgi.application'

# Database

# https://docs.djangoproject.com/en/4.1/ref/settings/#databases

DATABASES = {

   'default': {

       'ENGINE': 'django.db.backends.mysql',

       'NAME': 'elderco',

       'USER': 'root',

       'PASSWORD': 'password123',

       'HOST': 'localhost',

       'PORT': '3306',

   }

}

# Password validation

# https://docs.djangoproject.com/en/4.1/ref/settings/#auth-password-validators

AUTH_PASSWORD_VALIDATORS = [

   {

       'NAME': 'django.contrib.auth.password_validation.UserAttributeSimilarityValidator',

   },

   {

       'NAME': 'django.contrib.auth.password_validation.MinimumLengthValidator',

   },

   {

       'NAME': 'django.contrib.auth.password_validation.CommonPasswordValidator',

   },

   {

       'NAME': 'django.contrib.auth.password_validation.NumericPasswordValidator',

   },

]

# Internationalization

# https://docs.djangoproject.com/en/4.1/topics/i18n/

LANGUAGE_CODE = 'en-us'

TIME_ZONE = 'UTC'

USE_I18N = True

USE_TZ = True

# Static files (CSS, JavaScript, Images)

# https://docs.djangoproject.com/en/4.1/howto/static-files/

STATIC_URL = 'static/'

# Default primary key field type

# https://docs.djangoproject.com/en/4.1/ref/settings/#default-auto-field

DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'

Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm
$ ls
dcrm / manage.py*  website/
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm
$ clear 

Django Project – Code a CRM App Tutorial
website
mydb.py
# Install Mysql on your computer

# https://dev.mysql.com/downloads/installer/

# pip install mysql

# pip install mysql-connector

# pip install mysql-connector-python

import mysql.connector

dataBase = mysql.connector.connect(

	host = 'localhost',

	user = 'root',

	passwd = 'password123'

	)

# prepare a cursor object

cursorObject = dataBase.cursor()

# Create a database

cursorObject.execute("CREATE DATABASE elderco")

print("All Done!")

(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm
$ ls
dcrm manage.py* mydb.py website
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm
$ python mydb.py
All Done !
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm
$ clear

// python manage.py* migrate 

(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm
$ clear
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm
$ 

// python manage.py* create super user 

Username (leave blank to use ‘codemy’): admin
Email address:
Password:
Password (again ): 
Superuser Created successfully 

(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm
$ clear 

To run a server 
python manage.py* run server 
‘localhost:8000’


Django Version Control 

(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm
$ clear

https://codemy.com/git
$ git config --global user.name "Your Name"
$ git config --global user.email "you@youraddress.com"
$ git config --global push.default matching
$ git config --global alias.co checkout
$ git init

(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm
$ git config --global user.name “Rodrigo”
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm
$ git config --global user.email “rodrigomvsrodrigo@gmail.com”
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm
$ git config --global push.default matching
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm
$ git config --global alias.co checkout
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm
$ git init 
Initialized empty Git repository in C:/dcrm/dcrm/.git
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (master)
$ clear
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (master)
$ git add . 
(virt) 
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (master)
$ git commit -am ‘Initial Commit
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (master)
$ 


…or push an existing repository from the command line 
git remote add origin git@github.com:flatplanet/Django-CRM.git

(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (master)
$ git branch -M main
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (main)
$ git push -u origin main 
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (main)
$ 

https://github.com/flatplanet/Django-CRM

(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (main)
$ clear
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (main)
$  python manage.py runserver


DJANGO 
BUILD APP !

urls.py 
from django.urls import path
from . import views


urlpatterns = [
    path('', views.home, name='home'),
    #path('login/', views.login_user, name='login'),
    path('logout/', views.logout_user, name='logout'),
    path('register/', views.register_user, name='register'),
    path('record/<int:pk>', views.customer_record, name='record'),
    path('delete_record/<int:pk>', views.delete_record, name='delete_record'),
    path('add_record/', views.add_record, name='add_record'),
    path('update_record/<int:pk>', views.update_record, name='update_record'),


]

home.html 

{% extends 'base.html' %}

{% block content %}

{% if user.is_authenticated %}

// https://getbootstrap.com/docs/5.3/content/tables/

<table class="table table-striped table-hover table-bordered">

 <thead class="table-dark">

   <tr>

     <th scope="col">Name</th>

     <th scope="col">Email</th>

     <th scope="col">Phone</th>

     <th scope="col">Address</th>

     <th scope="col">City</th>

     <th scope="col">State</th>

     <th scope="col">Zipcode</th>

     <th scope="col">Created At</th>

     <th scope="col">ID</th>

   </tr>

 </thead>

 <tbody>

{% if records %}

	{% for record in records %}

		<tr>

			<td>{{ record.first_name }} {{ record.last_name }}</td>

			<td>{{ record.email }}</td>

			<td>{{ record.phone }}</td>

			<td>{{ record.address }}</td>

			<td>{{ record.city }}</td>

			<td>{{ record.state }}</td>

			<td>{{ record.zipcode }}</td>

			<td>{{ record.created_at }}</td>

			<td><a href="{% url 'record' record.id %}">{{ record.id }}</a></td>

		</tr>

	{% endfor %}

{% endif %}

	  </tbody>

	</table>

{% else %}

<div class="col-md-6 offset-md-3">

<h1>Login</h1>

<br/>

<form method="POST" action="{% url 'home' %}">

	{% csrf_token %}

 <div class="mb-3">

  <input type="text" class="form-control" name="username", placeholder="Username" required>

 </div><br/>

 <div class="mb-3">

   <input type="password" class="form-control" name="password", placeholder="Password" required>

 </div>

 <br/>

 <button type="submit" class="btn btn-secondary">Login</button>

</form>
{% endif %}

{% endblock %}

Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (main)
$  python manage.py runserver

base.html 
// https://getbootstrap.com/docs/introduction
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Django CRM</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-aFq/bzH65dt+w6FI2ooMVUpc+21e0SRygnTpmBvdBgSdnuTN7QbdgL+OapgHtvPp" crossorigin="anonymous">
  </head>
  <body>
   {% include’navbar.html’ %}
     <div class={“container”}>
     <br/>
            { %if messages% }
               { %for messages in message% }
                  <div class="alert alert-warning 
                  alert-dismissible fade show" role="alert">
           {{message}}
            <button type="button" class="btn-close" 
        data-bs-dismiss="alert" aria-label="Close"></
     button>
</div>

               {%endfor%}
           { %endif% }
            
{ % block content % }
{ % endblock % }
    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha2/dist/js/bootstrap.bundle.min.js" integrity="sha384-qKXV1j0HvMUeCBQ+QVp7JcfGl760yU08IQ+GpUo5hlbpg51QRiuqHAJz8+BrxE/N" crossorigin="anonymous"></script>
  </body>
</html>

navbar.html
//https://getbootstrap.com/docs/5.3/components/navbar/

<nav class="navbar navbar-expand-lg navbar-dark bg-dark">

 <div class="container-fluid">

   <a class="navbar-brand" href="{% url 'home' %}">Django CRM</a>

   <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">

     <span class="navbar-toggler-icon"></span>

   </button>

   <div class="collapse navbar-collapse" id="navbarSupportedContent">

     <ul class="navbar-nav me-auto mb-2 mb-lg-0">
       {% if user.is_authenticated %}

       <li class="nav-item">

         <a class="nav-link" href="{% url 'add_record' %}">Add Record</a>

       </li>

       <li class="nav-item">

         <a class="nav-link" href="{% url 'logout' %}">Logout</a>

       </li>

       {% else %}

       <li class="nav-item">

         <a class="nav-link" href="{% url 'register' %}">Register</a>

       </li>

       <li class="nav-item">

        <a class="nav-link" href="{% url 'home' %}">Login</a>

       </li>       

       {% endif %}
     </ul>
   </div>

 </div>

</nav>

DJANGO 
Login users

views.py
from django.shortcuts import render, redirect
from django.contrib.auth import authenticate, login, logout
from django.contrib import messages
from .forms import SignUpForm, AddRecordForm
from .models import Record

\\ localhost:8000/login/logout

def home(request):
	records = Record.objects.all()
	# Check to see if logging in
	if request.method == 'POST':
		username = request.POST['username']
		password = request.POST['password']
		# Authenticate
		user = authenticate(request, username=username, password=password)
		if user is not None:
			login(request, user)
			messages.success(request, "You Have Been Logged In!")
			return redirect('home')
		else:
			messages.success(request, "There Was An Error Logging In, Please Try Again...")
			return redirect('home')
	else:
		return render(request, 'home.html', {'records':records})



def logout_user(request):
	logout(request)
	messages.success(request, "You Have Been Logged Out...")
	return redirect('home')


def register_user(request):
	if request.method == 'POST':
		form = SignUpForm(request.POST)
		if form.is_valid():
			form.save()
			# Authenticate and login
			username = form.cleaned_data['username']
			password = form.cleaned_data['password1']
			user = authenticate(username=username, password=password)
			login(request, user)
			messages.success(request, "You Have Successfully Registered! Welcome!")
			return redirect('home')
	else:
		form = SignUpForm()
		return render(request, 'register.html', {'form':form})

	return render(request, 'register.html', {'form':form})



def customer_record(request, pk):
	if request.user.is_authenticated:
		# Look Up Records
		customer_record = Record.objects.get(id=pk)
		return render(request, 'record.html', {'customer_record':customer_record})
	else:
		messages.success(request, "You Must Be Logged In To View That Page...")
		return redirect('home')



def delete_record(request, pk):
	if request.user.is_authenticated:
		delete_it = Record.objects.get(id=pk)
		delete_it.delete()
		messages.success(request, "Record Deleted Successfully...")
		return redirect('home')
	else:
		messages.success(request, "You Must Be Logged In To Do That...")
		return redirect('home')


def add_record(request):
	form = AddRecordForm(request.POST or None)
	if request.user.is_authenticated:
		if request.method == "POST":
			if form.is_valid():
				add_record = form.save()
				messages.success(request, "Record Added...")
				return redirect('home')
		return render(request, 'add_record.html', {'form':form})
	else:
		messages.success(request, "You Must Be Logged In...")
		return redirect('home')


def update_record(request, pk):
	if request.user.is_authenticated:
		current_record = Record.objects.get(id=pk)
		form = AddRecordForm(request.POST or None, instance=current_record)
		if form.is_valid():
			form.save()
			messages.success(request, "Record Has Been Updated!")
			return redirect('home')
		return render(request, 'update_record.html', {'form':form})
	else:
		messages.success(request, "You Must Be Logged In...")
		return redirect('home')

DJANGO 
Logout users

urls.py
from django.urls import path

from . import views
urlpatterns = [

   path('', views.home, name='home'),

   #path('login/', views.login_user, name='login'),

   path('logout/', views.logout_user, name='logout'),

   path('register/', views.register_user, name='register'),

   path('record/<int:pk>', views.customer_record, name='record'),

   path('delete_record/<int:pk>', views.delete_record, name='delete_record'),

   path('add_record/', views.add_record, name='add_record'),

   path('update_record/<int:pk>', views.update_record, name='update_record'),

]

DJANGO
REGISTER USERS


register.html

{% extends 'base.html' %}

{% block content %}

<div class="col-md-6 offset-md-3">

<h1>Register</h1>

<br/>
<form method="POST" action="">

	{% csrf_token %}

	{% if form.errors %}

			<div class="alert alert-warning alert-dismissible fade show" role="alert">

			  Your Form Has Errors

			  {% for field in form %}


			  	{% if field.errors %}

			  	{{ field.errors }}

			  	{% endif %}

		 {% endfor %}

			  <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button>
			</div>
		{% endif %}
	{{ form.as_p }}
	<br/>

  <button type="submit" class="btn btn-secondary">Register</button>

	</form>
</div>
{% endblock %}

forms.py

from django.contrib.auth.forms import UserCreationForm

from django.contrib.auth.models import User

from django import forms

from .models import Record

class SignUpForm(UserCreationForm):

	email = forms.EmailField(label="", widget=forms.TextInput(attrs={'class':'form-control', 'placeholder':'Email Address'}))

	first_name = forms.CharField(label="", max_length=100, widget=forms.TextInput(attrs={'class':'form-control', 'placeholder':'First Name'}))

	last_name = forms.CharField(label="", max_length=100, widget=forms.TextInput(attrs={'class':'form-control', 'placeholder':'Last Name'}))

	class Meta:

	model = User

		fields = ('username', 'first_name', 'last_name', 'email', 'password1', 'password2')
	def __init__(self, *args, **kwargs):

		super(SignUpForm, self).__init__(*args, **kwargs)

		self.fields['username'].widget.attrs['class'] = 'form-control'

		self.fields['username'].widget.attrs['placeholder'] = 'User Name'

		self.fields['username'].label = ''

		self.fields['username'].help_text = '<span class="form-text text-muted"><small>Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only.</small></span>'
		self.fields['password1'].widget.attrs['class'] = 'form-control'

		self.fields['password1'].widget.attrs['placeholder'] = 'Password'

		self.fields['password1'].label = ''

		self.fields['password1'].help_text = '<ul class="form-text text-muted small"><li>Your password can\'t be too similar to your other personal information.</li><li>Your password must contain at least 8 characters.</li><li>Your password can\'t be a commonly used password.</li><li>Your password can\'t be entirely numeric.</li></ul>
		self.fields['password2'].widget.attrs['class'] = 'form-control'

		self.fields['password2'].widget.attrs['placeholder'] = 'Confirm Password'

		self.fields['password2'].label = ''

		self.fields['password2'].help_text = '<span class="form-text text-muted"><small>Enter the same password as before, for verification.</small></span>'	

# Create Add Record Form

class AddRecordForm(forms.ModelForm):

	first_name = forms.CharField(required=True, widget=forms.widgets.TextInput(attrs={"placeholder":"First Name", "class":"form-control"}), label="")
	last_name = forms.CharField(required=True, widget=forms.widgets.TextInput(attrs={"placeholder":"Last Name", "class":"form-control"}), label="")
email = forms.CharField(required=True, widget=forms.widgets.TextInput(attrs={"placeholder":"Email", "class":"form-control"}), label="")

	phone = forms.CharField(required=True, widget=forms.widgets.TextInput(attrs={"placeholder":"Phone", "class":"form-control"}), label="")

	address = forms.CharField(required=True, widget=forms.widgets.TextInput(attrs={"placeholder":"Address", "class":"form-control"}), label="")

	city = forms.CharField(required=True, widget=forms.widgets.TextInput(attrs={"placeholder":"City", "class":"form-control"}), label="")

	state = forms.CharField(required=True, widget=forms.widgets.TextInput(attrs={"placeholder":"State", "class":"form-control"}), label="")

	zipcode = forms.CharField(required=True, widget=forms.widgets.TextInput(attrs={"placeholder":"Zipcode", "class":"form-control"}), label="")

	class Meta:

model = Record

		exclude = ("user",)
  
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (main)
$ git add .
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (main)
$ git commit -am ‘registration’
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (main)
$ git push 
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (main)
$ python manage.py runserver


DJANGO
DATABASE MODEL

models.py

from django.db import models

class Record(models.Model):

	created_at = models.DateTimeField(auto_now_add=True)

	first_name = models.CharField(max_length=50)

	last_name =  models.CharField(max_length=50)

	email =  models.CharField(max_length=100)

	phone = models.CharField(max_length=15)

	address =  models.CharField(max_length=100)

	city =  models.CharField(max_length=50)

	state =  models.CharField(max_length=50)

	zipcode =  models.CharField(max_length=20)
	def __str__(self):

		return(f"{self.first_name} {self.last_name}")

(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (main)
$ clear
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (main)
$ python manage.py makemigrations
Migrations for ‘website’:
website\migrations\0001_inicial.py
Create model Record
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (main)
$ python manage.py migrate
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (main)
$ python manage.py runserver

admin.py

from django.contrib import admin

from .models import Record

admin.site.register(Record)

DJANGO 
VIEW RECORDS ON WEBSITE

{% extends 'base.html' %}

{% block content %}

<div class="col-md-6 offset-md-3">
<h1>Register</h1>

<br/>

<form method="POST" action="">

	{% csrf_token %}

	{% if form.errors %}

			<div class="alert alert-warning alert-dismissible fade show" role="alert">

			  Your Form Has Errors

			  {% for field in form %}

			  	{% if field.errors %}

			  		{{ field.errors }}

			  	{% endif %}
			  {% endfor %}
			  <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button>
			</div>
		{% endif %}
	{{ form.as_p }}
	<br/>
	  <button type="submit" class="btn btn-secondary">Register</button>
	</form>
</div>

{% endblock %}


DJANGO 
BOOTSTRAP TABLE

https://getbootstrap.com/docs/5.3/content/tables/

DJANGO 
INDIVIDUAL RECORDS

record.html
{% extends 'base.html' %}
{% block content %}



<div class="card">
  <div class="card-header"><strong>
    	{{ customer_record.first_name }} 
		{{ customer_record.last_name }}</strong>
  </div>
  <div class="card-body">



<p class="card-text">
<strong>Email: </strong>{{ customer_record.email }}</p>

<p class="card-text">
<strong>Phone: </strong>{{ customer_record.phone }}
</p>

<p class="card-text">
<strong>Address: </strong>{{ customer_record.address }}</p>

<p class="card-text">
<strong>City: </strong>{{ customer_record.city }}</p>

<p class="card-text">
<strong>State: </strong>{{ customer_record.state }}</p>

<p class="card-text">
<strong>Zipcode: </strong>{{ customer_record.zipcode }}</p>

<p class="card-text">
<strong>Create At: </strong>{{ customer_record.created_at }}</p>

<p class="card-text">
<strong>ID: </strong>{{ customer_record.id }}</p>
    
    
  </div>
</div>

<br/><br/>
<a href="{% url 'home' %}" class="btn btn-secondary">Back</a>

<a href="{% url 'delete_record' customer_record.id %}" class="btn btn-danger">Delete</a>

<a href="{% url 'update_record' customer_record.id %}" class="btn btn-secondary">Update Record</a>
		

{% endblock %}

DJANGO 
BOOTSTRAP CARD
record.html

{% extends 'base.html' %}

{% block content %}

<div class="card">

 <div class="card-header"><strong>

   	{{ customer_record.first_name }}

		{{ customer_record.last_name }}</strong>

 </div>

 <div class="card-body">

<p class="card-text">

<strong>Email: </strong>{{ customer_record.email }}</p>

<p class="card-text">

<strong>Phone: </strong>{{ customer_record.phone }}

</p>

<p class="card-text">

<strong>Address: </strong>{{ customer_record.address }}</p>

<p class="card-text">

<strong>City: </strong>{{ customer_record.city }}</p>

<p class="card-text">

<strong>State: </strong>{{ customer_record.state }}</p>

<p class="card-text">

<strong>Zipcode: </strong>{{ customer_record.zipcode }}</p>

<p class="card-text">
<strong>Create At: </strong>{{ customer_record.created_at }}</p>

<p class="card-text">

<strong>ID: </strong>{{ customer_record.id }}</p>

 </div>

</div>

<br/><br/>

<a href="{% url 'home' %}" class="btn btn-secondary">Back</a>

<a href="{% url 'delete_record' customer_record.id %}" class="btn btn-danger">Delete</a>

<a href="{% url 'update_record' customer_record.id %}" class="btn btn-secondary">Update Record</a>

{% endblock %}


DJANGO 
DELETE RECORD 

urlsl.py

DJANGO 
ADD RECORDS

urlsl.py

add.record.html
{% extends 'base.html' %}
 
{% block content %}

<div class="col-md-6 offset-md-3">

<h1>Add Record</h1>

<br/>

<form method="POST" action="{% url 'add_record' %}">

	{% csrf_token %}

	{{ form.as_p }}
<br/>

 <button type="submit" class="btn btn-secondary">Add Record</button>

  <a href="{% url 'home' %}" class="btn btn-secondary">Back</a>
</form>
</div>
{% endblock %}


DJANGO
UPDATE RECORDS

update_record.html
{% extends 'base.html' %}
{% block content %}

<div class="col-md-6 offset-md-3">
<h1>Add Record</h1>
<br/>

<form method="POST">
	{% csrf_token %}

	{{ form.as_p }}

<br/>
  <button type="submit" class="btn btn-secondary">Update Record</button>

</form>


</div>

{% endblock %}


DJANGO 
PUSH CODE TO GITHUB.COM

(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (master)
$ git branch -M main
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (main)
$ git push -u origin main 
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (main)
$ git add .
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (main)
$ git commit -am ‘Final Project’
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (main)
$ git push 
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (main)
$ python manage.py runserver
(virt)
Matheus@DESKTOP-3OTOCA6 MINGW64 /c/dcrm/dcrm (main)
$ 


