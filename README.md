# Django Blog Demo

## About

This repository made using **Python 3.11** + **Django**, database provided by **SQLite**,
**Bootstrap** was used for styling, and testing is done using **untitest** module.

There is a login and registration functionality included.

User has his own blog page, where he can add new blog posts. 
Every authenticated user can comment on posts made by other users.
Home page is paginated list of all posts.
Non-authenticated users can see all blog posts, but cannot add new posts or comment.

App is covered with tests.

## Prerequisites

\[Optional\] Install and activate virtual environment using either venv or conda.

### venv

```bash
$ python -m virtualenv env
$ source env/bin/activate
```

### conda
```bash
conda create -n djangoblog python=3.10
conda activate djangoblog
```

Install dependencies:
```bash
$ pip install -r requirements.txt
```

## How to run

### Default

You can run the application from the command line with manage.py. 

Go to the root folder of the application and run the following script.

```
$ chmod +x scripts/run.sh
$ scripts/run.sh
```

## Post Installation

Go to the web browser and visit `http://localhost:8000/blog`

Admin username: **admin**
Admin password: **adminpassword**
User username: **dusan**
User password: **dusanpassword**

## Helper Tools

### Django Admin

It is possible to add additional admin user who can login to the admin site. Run the following command:
```bash
$ python manage.py createsuperuser
```
Enter your desired username and press enter.
```bash
Username: admin_username
```
You will then be prompted for your desired email address:
```bash
Email address: admin@example.com
```
The final step is to enter your password. You will be asked to enter your password twice, the second time as a confirmation of the first.
```bash
Password: **********
Password (again): *********
Superuser created successfully.
```

Go to the web browser and visit `http://localhost:8000/admin`

### Tests
```bash
$ python manage.py test blog
```