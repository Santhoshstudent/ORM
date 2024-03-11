# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
...
admin.py
from django.contrib import admin
from .models import Footballplayer,FootballplayerAdmin
admin.site.register(Footballplayer,FootballplayerAdmin)

models.py
from django.db import models
from django.contrib import admin
class Footballplayer(models.Model):
    name=models.CharField(max_length=20)
    role=models.CharField(max_length=10)
    age=models.IntegerField()
    experience=models.IntegerField()
    country=models.CharField(max_length=20)

class FootballplayerAdmin(admin.ModelAdmin):
    list_display=('name','role','age','experience','country')
...



## OUTPUT

![web ocm](https://github.com/Santhoshstudent/ORM/assets/145446853/c0c8cb08-9179-4914-8962-1e3c0e8fe0ca)



## RESULT
