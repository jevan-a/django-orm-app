# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![employee list](https://user-images.githubusercontent.com/103949835/210123393-e10845d3-4027-4d9d-96f3-b21ad80de2af.png)


## DESIGN STEPS

### STEP 1:
First go to student.saveetha.ac.in and open theiaIDE

### STEP 2:
Open theiaIDE and go to admin.py and open models.py put some comments

### STEP 3:
Open github.com and create and generate classic token 

Write your own steps

## PROGRAM
python
~~~
class Employee(models.Model):
    emp_id=models.CharField(primary_key=True,max_length=4,help_text="Employee ID")
    ename=models.CharField(max_length=50)
    post=models.CharField(max_length=20)
    salary=models.IntegerField()
    age=models.IntegerField()


class EmployeeAdmin(admin.ModelAdmin):
    list_display=('emp_id','ename','post','salary','age')
    
~~~

python
~~~
from django.db import models
from django.contrib import admin
# Register your models here.
admin.site.register(Employee,EmployeeAdmin)


~~~
# Create your models here.




## OUTPUT

![employee details](https://user-images.githubusercontent.com/103949835/210123410-a6cae3a4-0936-4b95-82c0-61b165dcd525.png)


![employee error](https://user-images.githubusercontent.com/103949835/210123405-e1468439-579a-4d87-a6a6-6090fa75bda7.png)



## RESULT
I  developed a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).
