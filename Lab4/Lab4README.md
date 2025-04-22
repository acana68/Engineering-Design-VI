# Lab 4 – Django Web Framework (CPE 322)

This lab demonstrates setting up and running a basic Django application using Python. The goal was to install Django, configure project settings, create a minimal web app, and verify functionality through a browser.

---

## Installation & Setup Steps

### 1. Installed Required Packages
```bash
pip3 install -U django djangorestframework django-filter markdown requests
```
![step1](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab4/lab4%231.png?raw=true)  
![step2](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab4/lab4%232.png?raw=true)  
![step3](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab4/lab4%233.png?raw=true)  

---

### 2. Created Project and App
```bash
django-admin startproject stevens
cd stevens
python manage.py startapp myapp
```
![step4](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab4/lab4%234.png?raw=true)  
![step5](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab4/lab4%235.png?raw=true)  

---

### 3. Updated settings.py
- Added `'myapp'` to `INSTALLED_APPS`
- Set `ALLOWED_HOSTS = ['*']`
- Set `TIME_ZONE = 'America/New_York'`

![step6](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab4/lab4%236.png?raw=true)  
![step7](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab4/lab4%237.png?raw=true)  

---

### 4. Created View in myapp/views.py
```python
from django.http import HttpResponse

def index(request):
    return HttpResponse("Hello from my IoT Django app!")
```
![step8](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab4/lab4%238.png?raw=true)  

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
![step9](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab4/lab4%239.png?raw=true)  

**stevens/urls.py**
```python
from django.contrib import admin
from django.urls import path, include

urlpatterns = [
    path('admin/', admin.site.urls),
    path('', include('myapp.urls')),
]
```
![step10](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab4/lab4%2310.png?raw=true)  

---

### 6. Ran Server and Verified Output
```bash
python manage.py runserver
```
![step11](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab4/lab4%2311.png?raw=true)  
![step12](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab4/lab4%2312.png?raw=true)  

---

## Conclusion

All required packages were installed successfully. The Django application was created, configured, and verified through browser output. The basic view and URL routing are functional, completing the required portion of Lab 4.
