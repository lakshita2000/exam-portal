# exam-portal
Exam Portal In Django
# Live Website -> https://exam-portal-django.herokuapp.com/
# Please Note: On live website users cannot create professor accounts
# Main Features:
# Auto Submit Form as soon as timer runs out
# If student window goes out of focus for 5 times while appearing for an exam professor will receive an email
# Automatic calculation of marks once student submits Exam
# To run this project follow the instructions given below:
# Please Note: Python 3.8.2 is needed to run this project
# First Clone the project
# git clone https://github.com/lakshita2000/exam-portal.git
# cd Exam-Portal
# Now we will need a .env file for storing email credentials
  # create .env in the Exam-Portal directory
   # Contents of .env file
   # export EMAIL_HOST_PASSWORD=<PASSWORD_OF_EMAIL_ACCOUNT>
   # export EMAIL_HOST_USER=<EMAIL_ACCOUNT>
   # export EMAIL_HOST
After creating env file, run following commands:-

# cd Exam
# python manage.py migrate
# python manage.py makemigrations
# python manage.py migrate
Once done with that create a superuser account:
# python manage.py createsuperuser
Once superuser account is created we can run the website
# python manage.py runserver
# If there are no errors website will be running on http://127.0.0.1:8000/ (default)
For creating accounts for professor's we will need a group called Professor
Go to http://127.0.0.1:8000/admin/auth/group/add/
Login with superuser account
Add a new group named Professor
For Professor verification, admin will need to manually add professor to Professor group once they create a new account
