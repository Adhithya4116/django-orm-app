# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![entity](https://user-images.githubusercontent.com/118707079/215281822-cfe034fd-a721-4ed6-9d3e-56ae27474c8f.png)


Step 1:
create and collect customers infomartion using django application

Step 2:
Implement that as Python code

Step 3:
push that python code to github

## PROGRAM
```
from django.db import models

# Create your models here. 
from django.db import models
from django.contrib import admin
# Create your models here.
class Customer(models.Model):
    customerid = models.CharField(max_length=8,primary_key=True)
    customername =models.CharField(max_length=100)
    mobilenumber =models.CharField(max_length=100)
    email = models.EmailField()
    quantity= models.IntegerField()
    

class CustomerAdmin(admin.ModelAdmin):
    list_display = ('customerid','customername','mobilenumber','email','quantity')
    
```
    
##OUTPUT

![table](https://user-images.githubusercontent.com/118707079/215283317-970fbb13-2d4b-451e-ab5b-f30493a078de.png)

![djangooutput](https://user-images.githubusercontent.com/118707079/215283291-1b794ef7-5479-4cdf-8126-f4b7ede219f3.png)

## RESULT
The program was executed Successfully.

