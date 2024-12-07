# Ex02 Django ORM Web Applicatio
# Date:18/10/2024
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

models.py
from django.db import models
from django.contrib import admin
class Bankloan (models.Model):
    Customer_ID=models.IntegerField(primary_key=True)
    Customer_Name=models.CharField(max_length=100)
    Customer_Salary=models.IntegerField()
    Customer_Age=models.IntegerField()
    Req_Loan_Amt=models.IntegerField()
 
class LoanAdmin(admin.ModelAdmin):
    list_display=('Customer_ID','Customer_Name','Customer_Salary','Customer_Age','Req_Loan_Amt')

admin.py

from django.contrib import admin
from .models import Bankloan,LoanAdmin
admin.site.register(Bankloan,LoanAdmin)

```
# OUTPUT
Include the screenshot of your admin page.

![Screenshot 1](https://github.com/user-attachments/assets/31071ea5-4645-4f57-b0cf-153144d15318)

![screenshot 2](https://github.com/user-attachments/assets/f8e35347-7d76-4282-8d4c-f1c8670de2eb)

![screenshot 3](https://github.com/user-attachments/assets/b33c283d-eb4b-41a4-b4c2-f7db56173d33)




# RESULT
Thus the program for creating a database using ORM hass been executed successfully
