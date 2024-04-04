# Ex02 Django ORM Web Application

## Date: 04/04/2024

## AIM:
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram:
![image](https://github.com/Yugendaran/ORM/assets/128135616/f5dfe3f8-0c52-49ea-b025-9bd9d07dd816)



## DESIGN STEPS:

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM:
admin.py:
```
from django.contrib import admin

from .models import Train, TrainAdmin

admin.site.register(Train, TrainAdmin)
```
models.py:
```
from django.db import models
from django.contrib import admin
class Train(models.Model):
    Train_code=models.CharField(max_length=20,primary_key=True)
    Train_name=models.CharField(max_length=100)
    start_time=models.TimeField()
    End_time=models.TimeField()
    start_station_code=models.CharField(max_length=20)
    End_station_code=models.CharField(max_length=20)
 
class TrainAdmin(admin.ModelAdmin):
    list_display=('Train_code','Train_name','start_time','End_time','start_station_code','End_station_code')
```
## OUTPUT:
![image](https://github.com/Yugendaran/ORM/assets/128135616/af53b799-3107-42c6-afbd-2db1f1037d33)

![image](https://github.com/Yugendaran/ORM/assets/128135616/7d45ca65-7913-43e5-b062-d6a6ab920c81)



## RESULT:
Thus the program for creating a database using ORM hass been executed successfully.

