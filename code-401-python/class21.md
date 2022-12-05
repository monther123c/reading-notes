# Django Custom User
---
Django ships with a built-in User model for authentication and if you’d like a basic tutorial on how to implement log in, log out, sign up and so on see the Django Login and Logout tutorial for more.

However, for a real-world project, the official Django documentation highly recommends using a custom user model instead. This provides far more flexibility down the line so, as a general rule, always use a custom user model for all new Django projects.

But how to implement one? The official documentation example is not actually what many Django experts recommend using. There is a far easier yet still powerful approach to starting off new Django projects with a custom user model which I’ll demonstrate here.

---
##  Setup To start, create a new Django project from the command line. We need to do several things:
1- create and navigate into a dedicated directory called accounts for our code

2- install Django

3- make a new Django project called django_project

4- make a new app accounts

5- start the local web serve

---
- AbstractUser vs AbstractBaseUser If you need full control over User model, it is better to use AbstractBaseUser but if you are just adding things to the existing user, for example, you just want to add an extra field bio ,location field or any other profile data then use AbstractUser.

---
- Superuser It's helpful to create a superuser that we can use to log in to the admin and test out log in/log out python manage.py createsuperuser