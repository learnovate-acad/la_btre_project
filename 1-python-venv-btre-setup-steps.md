# Step 1 
python3 -m venv ./venv

# Step 2
pip install django

# Step 3
django-admin help

# step 4
django-admin startproject btre .

# step 4
python manage.py help

# step 5

Cmd Shitp P > Select Python Intrepreter (or) Bottom Tool Bar Left Side change to ./venv/bin/python

When asked for Python Linter (pylint), install

# Step 6
pip freeze

Output :
asgiref==3.2.7
astroid==2.3.3
Django==3.0.5
isort==4.3.21
lazy-object-proxy==1.4.3
mccabe==0.6.1
pylint==2.4.4
pytz==2019.3
six==1.14.0
sqlparse==0.3.1
wrapt==1.11.2

# Step 7
git init

# step 8
Goto http://gitignore.io/ and type django

Create .gitignore as per website file info at rrot folder
add venv/ to .gitignore file

# Step 9
git add .
git commit -m "Initial Commit"

git config --global user.name learnovate-acad
git config --global user.email learnovate.academy2019@gmail.com

# Step 10 Run Django Server

python manage.py runserver







