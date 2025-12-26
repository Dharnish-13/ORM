# Ex02 Django ORM Web Application
# Date:
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 cars

# PROGRAM
```
from django.db import models
from django.contrib import admin

class Loan(models.Model):
    loan_id = models.AutoField(primary_key=True)
    customer_name = models.CharField(max_length=100)
    loan_amount = models.DecimalField(max_digits=10, decimal_places=2)
    interest_rate = models.DecimalField(max_digits=5, decimal_places=2)
    loan_term = models.IntegerField()
    disbursement_date = models.DateField()

class LoanAdmin(admin.ModelAdmin):
list_display=('loan_id','customer_name','loan_amount','interest_rate','loan_term','disbursement_date')
```
# OUTPUT
<img width="1721" height="910" alt="Screenshot 2025-12-26 095437" src="https://github.com/user-attachments/assets/05c5410e-07fb-4ccd-8ddc-e2798bd1f670" />
<img width="1674" height="909" alt="Screenshot 2025-12-26 095458" src="https://github.com/user-attachments/assets/97ba82aa-583e-42e9-b76e-49dbac7bbae9" />

Include the screenshot of your admin page.

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
