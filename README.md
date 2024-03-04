# Ex02 Django ORM Web Application
## Date: 28/02/24

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## DESIGN STEPS

![WhatsApp Image 2024-03-04 at 13 17 51_057e2951](https://github.com/chandramohan3/ORM/assets/142579775/c2ef54a1-6887-4d07-a638-526e2ced3f25)


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

admim.py

from django.contrib import admin
from.models import Book_DB,Book_DBAdmin
admin.site.register(Book_DB,Book_DBAdmin)

models.py

from django.db import models
from django.contrib import admin
class Book_DB(models.Model):
    b_id = models.IntegerField(primary_key="b_id");
    b_name = models.CharField(max_length=100);
    b_author = models.CharField(max_length=100);
    b_edition = models.CharField(max_length=20);
    b_year = models.DateField();

class Book_DBAdmin(admin.ModelAdmin):
    list_display = ("b_id","b_name","b_author","b_edition","b_year");
    
```


## OUTPUT

![alt text](<Screenshot 2024-02-28 092112.png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
