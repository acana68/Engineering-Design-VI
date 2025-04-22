# Lab 4 – Django Web Framework (CPE 322)

This lab demonstrates setting up and running a basic Django application using Python. The goal was to install Django, configure project settings, create a minimal web app, and verify functionality through a browser.

---

## Installation & Setup Steps

### 1. Installed Required Packages
```bash
pip3 install -U django djangorestframework django-filter markdown requests
```
![lab4 step 1](lab4#1.png)  
![lab4 step 2](lab4#2.png)  
![lab4 step 3](lab4#3.png)  

---

### 2. Created Project and App
```bash
django-admin startproject stevens
cd stevens
python manage.py startapp myapp
```
![lab4 step 4](lab4#4.png)  
![lab4 step 5](lab4#5.png)  

---

### 3. Updated settings.py
- Added `'myapp'` to `INSTALLED_APPS`
- Set `ALLOWED_HOSTS = ['*']`
- Set `TIME_ZONE = 'America/New_York'`

![INSTALLED_APPS and ALLOWED_HOSTS](lab4#6.png)  
![TIME_ZONE](lab4#7.png)  

---

### 4. Created View in myapp/views.py
```python
from django.http import HttpResponse

def index(request):
    return HttpResponse("Hello from my IoT Django app!")
```
![views.py](lab4#8.png)

---

### 5. Created URL Mappings

**myapp/urls.py**
```python
from django.urls import path
from . import views

urlpatterns = [
    path('', views.index),
]
```
![myapp urls.py](lab4#9.png)

**stevens/urls.py**
```python
from django.contrib import admin
from django.urls import path, include

urlpatterns = [
    path('admin/', admin.site.urls),
    path('', include('myapp.urls')),
]
```
![stevens urls.py](lab4#10.png)

---

### 6. Ran Server and Verified Output
```bash
python manage.py runserver
```
![Browser output](lab4#11.png)  
![Server output](lab4#12.png)

---

## Conclusion

All required packages were installed successfully. The Django application was created, configured, and verified through browser output. The basic view and URL routing are functional, completing the required portion of Lab 4.
