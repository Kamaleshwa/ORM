# Ex02 Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a student database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![image](https://github.com/Kamaleshwa/ORM/assets/144980199/c33148ba-1780-418c-8e84-b2c13ddeb832)


## DESIGN STEPS

### STEP 1:
clone the respository from github

### STEP 2:
create on admin interface for django

### STEP 3:
create an folder and edit settings.py

### STEP 4:
makemigration and migrate the changes

### STEP 5:
create admin.py and write program for admin and models


## PROGRAM
```
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
```

## OUTPUT
![image](https://github.com/Kamaleshwa/ORM/assets/144980199/15a72bd9-ac74-406e-b95d-1fb24e262dfa)



## RESULT
The program  for creating student database using ORM is successful
