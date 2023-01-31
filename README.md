# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

# DESIGN STEPS
# STEP 1:
Clone the problem from github

# STEP 2:
create a new app

# STEP 3:
Enter the code for admin.py and model.py

# STEP 4:
Execute Django admin and create 10 employees

# PROGRAM:
```
Model.py
from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,help_text="Employee ID")
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')

 Admin.py

   from django.contrib import admin
from .models import Employee,EmployeeAdmin
# Register your models here.
admin.site.register(Employee,EmployeeAdmin) 
```
## OUTPUT

     
     
     ![Screenshot (122)](https://user-images.githubusercontent.com/119476069/215653028-0f99f7ba-9ca0-4096-b528-0816878b6bad.png)

     


## RESULT
The django ORM is executed successfully
