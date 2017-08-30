# My-first-blog
01. Download the files to your Computer. Download and install Python 3 in your system for Windows. Make sure "pip" gets installed as well.
02. Open the cmd in Windows and go to the location where the above files are stored. Eg, if the path is "C:\Django\myFirstSite", go to         "C:\Django".
03. Install Django 1.11 using command "pip install django".
04. Install virtual environment using command "python -m venv myvenv".
05. Download and install PostgreSQL 9.6 for Windows. During installation, you will be asked for a password. Enter 'admin' as password as       it is hard coded. Choose a location where you want to store your database. Its preferable to leave it blank for the default location.
06. In the cmd, type "psql -U postgres" to enter PostgreSQL inerface. Enter the password you submitted in step 5.
07. Create a user using command "CREATE USER admin;". User name should be 'admin' only as it is hard coded.
08. Create a database using command "CREATE DATABASE blog OWNER admin;". Database name should be 'blog' only as it is hard coded.
09. Exit the postgreSQL interface by pressing Ctrl+c keys.
10. Start virtual environment by typing "myvenv\Scripts\activate" in cmd. Make sure there is a folder named myvenv created in path             "C:\Django" from Step 4. Virtualenv will isolate your Python/Django setup on a per-project basis. This means that any changes you make     to one website won't affect any others you're also developing. Type "cd myFirstSite" in the cmd to go to "C:\Django\myFirstSite". 
11. Type "django-admin createsuperuser" in cmd to create a super user who has admin rights for Django admin page. Provide the required         details and remember the password.
12. Install psycopg2 using command "pip install psycopg2". It provides connectivity between Python and PostgreSQL.
13. Install social auth using command "pip install django-social-auth". It is a package that allows login from social websites.
14. Type "python manage.py makemigrations" to create the database structure in PostgreSQL. Then type "python manage.py migrate". Now you       have a database structure for the blog application.
15. To run the server type "python manage.py runserver". Now go to Chrome browser and type 127.0.0.1:8000 as URL. Voila!!!
16. For login purpose, you can either use gmail credentials or Django admin credentials you created in Step 11.
