[Back to Home](../README.md)

## Reading Class-32: Permissions & Postgresql

**1. Django Rest Framework (DRF) Permissions:**

DRF provides components for securing APIs:
- **Authentication:** Identifies users making requests.
- **Permissions:** Controls user access based on actions and roles.
- **Authorization:** Ensures users manipulate only allowed data.
- **View-Level Permissions:** Define permissions for specific views.

**2. SQL SELECT statement for retrieving all columns from 'employees' table:**

To fetch all columns from 'employees':
```sql
SELECT *
FROM employees;
```

**3. DRF Generic Views:**

Pre-built views for common API operations:
- **ListAPIView:** Retrieve a list of objects.
- **RetrieveAPIView:** Retrieve a single object by PK.
- **CreateAPIView:** Create a new object.
- **UpdateAPIView:** Update an existing object.
- **DestroyAPIView:** Delete an object.

Example:

```python
from rest_framework.generics import ListAPIView, RetrieveAPIView, CreateAPIView, UpdateAPIView, DestroyAPIView
from .models import Employee
from .serializers import EmployeeSerializer

class EmployeeListView(ListAPIView):
    queryset = Employee.objects.all()
    serializer_class = EmployeeSerializer

class EmployeeDetailView(RetrieveAPIView):
    queryset = Employee.objects.all()
    serializer_class = EmployeeSerializer

class EmployeeCreateView(CreateAPIView):
    queryset = Employee.objects.all()
    serializer_class = EmployeeSerializer

class EmployeeUpdateView(UpdateAPIView):
    queryset = Employee.objects.all()
    serializer_class = EmployeeSerializer

class EmployeeDestroyView(DestroyAPIView):
    queryset = Employee.objects.all()
    serializer_class = EmployeeSerializer
```

Using DRF Generic Views simplifies API development and adheres to RESTful principles.

*- Author: Almothana Almasri*