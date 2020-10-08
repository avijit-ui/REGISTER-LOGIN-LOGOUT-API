# REGISTER-LOGIN-LOGOUT-API
REGISTER-LOGIN-LOGOUT-API source code

INTRODUCTION

This project of Register-Login-Logout and Change Password API is designed by django Rest framework and django.

This is a Register-Login-Logout and Change Password API.In this API you will find user registration,login,logout,change password features.We have used token based authentication.
For user registration -
If a user writes this link in the browser's address bar 'http://localhost:8000/api/register/',the user can get registered by given the proper credentials.After registration the user
will get the credentials except the password field with token.This process can also be done by postman,there the method must be post.
For user login-
In Postman User can give the credentials using either json format or in key-value pair.In postman write in the request url 'http://localhost:8000/api/login/',method will be post
and in the body section the user will give the username and password,and in the response you will get the token and expiry.

For user logout-
In postman the user write in the request url 'http://localhost:8000/api/logout/',method will be post and Add the authorization token in the headers section which the user get 
during login.In the response the user will get status:204 No Content that means the login user is now logged out.  



for change password-
If a user wants to change the password.In postman add the authorization token which the user get during login in the headers authorization field .method will be put and in the body
section the user will give the old password and new password.In the response the user will get the the successful message.

Technologies

Django==3.1.1
django-rest-knox==4.1.0
djangorestframework==3.11.1
psycopg2==2.8.6

Launch

To run this project locally,install 'requirements.txt' file using pip: cd RegisterLoginLogoutAPI pip install requirements.txt

