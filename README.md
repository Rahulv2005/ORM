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
admin.py
from django.contrib import admin
from .models import student,studentAdmin
admin.site.register(student,studentAdmin)

models.py
from django.db import models
from django.contrib import admin
class student (models.Model):
    name=models.CharField(max_length=20,help_text="student")
    rollno=models.IntegerField()
    refno=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
class studentAdmin(admin.ModelAdmin):
    list_display=('name','rollno','refno','age','email')

## OUTPUT

![image](https://github.com/Rahulv2005/ORM/assets/152600335/54693175-6d95-4042-9de4-8dba0bd69ab2)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
