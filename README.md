# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clonining of repository.Setting up of admin models


### STEP 2:
To make all migrations in the app.Test the server.

### STEP 3:
Include the detials in the tables.

Write your own steps

## PROGRAM
models.py:
``` python
from django.db import models
from django.contrib import admin
class Employee(models.Model):
    emp_id=models.CharField(primary_key=True,max_length=4,help_text="Employee ID")
    ename=models.CharField(max_length=50)
    post=models.CharField(max_length=50)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('emp_id','ename','post','salary','age','email')  
```
 admin.py:
```
from django.contrib import admin
from .models import Employee,EmployeeAdmin

# Register your models here.
admin.site.register(Employee,EmployeeAdmin) 
```

Include your code here

## OUTPUT
###DJANGO
![output](/3e121d92-ecd7-4b9c-a0ec-353127cc2007.jpeg)
###primary key
![output](/8c399347-194f-4465-8e4d-8ceee4fc78e4.jpeg)

Include the screenshot of your admin page.


## RESULT
Thus we delveloped a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).