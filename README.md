# Ex02 Django ORM Web Application
# Date:18-10-2024
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
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
from django.db import models
from django.contrib import admin

class BankLoan(models.Model):
    acc = models.IntegerField(primary_key=True)  
    ph = models.IntegerField()  
    ifsc = models.CharField(max_length=100)  
    loanno = models.IntegerField()  
    address = models.CharField(max_length=100) 
    pan = models.IntegerField()  
    adhar = models.IntegerField()
admin.py:
from django.contrib import admin

from .models import BankLoan, BankLoanAdmin
  

class BankLoanAdmin(admin.ModelAdmin):
    list_display = ('acc', 'ph', 'ifsc', 'loanno', 'address', 'pan', 'adhar')


admin.site.register(BankLoan, BankLoanAdmin)
```

# OUTPUT
Include the screenshot of your admin page.
![group mem](https://github.com/user-attachments/assets/e4330198-07c1-4490-aeaa-dc0cfbf90fd3)




![Screenshot 2024-12-07 105523 user](https://github.com/user-attachments/assets/80e53117-c737-4c55-ada4-451e9c67399a)




![Screenshot 2024-12-07 105604 bank lone](https://github.com/user-attachments/assets/9c26140a-72d7-4b68-ab4a-39f04cc9c119)




# RESULT
Thus the program for creating a database using ORM hass been executed successfully
