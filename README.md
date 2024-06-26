# Ex02 Django ORM Web Application
## Date: 13.03.24

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![WhatsApp Image 2024-03-21 at 19 51 57_a1b0389b](https://github.com/23013633/ORM/assets/150005961/1707882a-baf2-419f-8df4-91e607a5a7a3)



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
```
admin.py

from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

models.py
from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,primary_key=True)
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
 
class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')

```



## OUTPUT
![Screenshot 2024-03-13 211731](https://github.com/23013633/ORM/assets/150005961/0b5a2b90-8c0e-48d8-9f37-00c8a9733c3d)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
