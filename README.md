# Ex02 Django ORM Web Application
# Date: 
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM

![Screenshot 2024-12-06 213233](https://github.com/user-attachments/assets/f4b50d3a-ded2-4ddb-ad14-960c154d08cb)

## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
```
models.py

from django.db import models                                                                                                                      
from django.contrib import admin                                             
class book(models.Model):                    				      
   bookno=models.IntegerField(primary_key=True);                                                      
   authorname=models.CharField(max_length=50);                                                            
   price=models.IntegerField(help_text="enter price");                       
   qty=models.IntegerField();                                                
   bookname=models.CharField(max_length=50);                                 
class bookAdmin(admin.ModelAdmin):                                           
   list_display=("bookno","authorname","price","qty","bookname"); 

admin.py

from django.contrib import admin                                             
from .models import book,bookAdmin                                           
admin.site.register(book,bookAdmin)
```
# OUTPUT

![Screenshot 2024-12-06 213209](https://github.com/user-attachments/assets/28f4eca8-9058-48d5-8d94-edd309f8803a)

![Uploading user.jpg…]()

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
