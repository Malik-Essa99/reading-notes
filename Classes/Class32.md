## Class 32

### Q1. What are the key components and purpose of Django Rest Framework (DRF) permissions, and how do they help in securing an API?

Django Rest Framework (DRF) permissions are a vital feature that helps secure your API by controlling access to resources and actions. They work in conjunction with authentication to enforce restrictions and provide authorization mechanisms. The key components and purpose of DRF permissions are as follows:

1. Authentication
2. Authorization
3. Permission Classes
4. permission_classes attribute

DRF permissions help secure your API by:

+ Controlling Access: They allow you to define who can access specific API endpoints, ensuring that only authorized users have access to protected resources.

+ Preventing Unauthentfgicated Access: DRF permissions, such as IsAuthenticated, prevent unauthenticated users from accessing sensitive data and operations.

+ Fine-Grained Authorization: Custom permission classes enable you to implement fine-grained access control based on user roles, ownership, group membership, or any other criteria.

+ Consistent Security: DRF permissions provide a standardized way to handle authentication and authorization, promoting consistent security practices across your API.

---

### Q2. In SQL, what is the purpose of the SELECT statement, and how would you use it to retrieve all columns from a table called ‘employees’?

SELECT statement is a fundamental query used to fetch data from a database. Its primary purpose is to retrieve specific columns or expressions from one or more tables based on certain conditions or criteria.
Example: 

+ Select * from table

---

### Q3. Can you explain the role of DRF Generic Views and provide examples of their usage in building a RESTful API?

Django Rest Framework (DRF) Generic Views provide a set of pre-built view classes that simplify the process of building RESTful APIs. They cover common actions like listing, retrieving, creating, updating, and deleting objects from a database. By utilizing DRF Generic Views, developers can significantly reduce code duplication and accelerate API development. The process involves creating serializers to handle data serialization/deserialization and defining view classes that utilize DRF's Generic Views to perform CRUD operations on models. With minimal code, DRF Generic Views enable the creation of powerful and consistent RESTful APIs.


Assuming we already created snacks app, in views.py file:

``` 
from rest_framework import generics
from .models import Snack
from .serializers import SnackSerializer

class SnackListView(generics.ListCreateAPIView):
    queryset = Snack.objects.all()
    serializer_class = BookSerializer

class SnackDetailView(generics.RetrieveUpdateDestroyAPIView):
    queryset = Snack.objects.all()
    serializer_class = BookSerializer

```