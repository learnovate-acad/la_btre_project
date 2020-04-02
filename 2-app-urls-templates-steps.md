# Intsall Python Formatter autopep8 (in virtual env)
pip install autopep8

### Create a new application in Django 

# Step 1  (in virtual env)
python manage.py startapp pages

(Look for folder Pages created by prev command)

# Step 2 - Register Pages App to settings.py of btre Project
INSTALLED_APPS = [
    'pages.apps.PagesConfig',

Check with pip freeze

# Step 3 : For setting up pages app as route
## Create urls.py in pages folder 
## Now check the content written in urls.py and views.py
### urls.py

from django.urls import path

from . import views

urlpatterns = [
    path('', views.index , name = 'index')
]

### views.py

from django.shortcuts import render

from django.http import HttpResponse

def index(request):
    return HttpResponse('<h1>Hello World</h1>')

# Step 4 : Associate pages urls.py to btre folder urls.py

from django.contrib import admin
from django.urls import path, include

urlpatterns = [
    # DO not use '/' for home page instead use ''
    path('', include('pages.urls')),
    path('admin/', admin.site.urls),
]

# Set up Layouts

# Step 1 : In settings.py - Specify Templates folder

TEMPLATES = [
    {
        'BACKEND': 'django.template.backends.django.DjangoTemplates',
        'DIRS': [os.path.join(BASE_DIR, 'templates')],

