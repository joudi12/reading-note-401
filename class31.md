# summery 
## Python Docker
![image](https://miro.medium.com/max/551/0*b_b7YNPHXalG21LW.jpeg)
### Docker is a containerization tool used for spinning up isolated, reproducible application environments. It is a popular development tool for Python developers.When you develop an application, you need to provide your code along with all possible dependencies like libraries, the web server, databases, etc. You may end up in a situation when the application is working on your computer, but won’t even start on the staging server, or the dev or QA’s machine.This challenge can be addressed by isolating the app to make it independent of the system

## Docker vs Virtual Environments
### Virtual environments are used to isolate Python software packages locally. We can create an isolated box for individual projects so one can use Python 2.7 and Django 1.5 while another can use Python 3.5 and Django 2.1 on the same computer. Virtual environments are great.

### But…virtual environments can only isolate Python packages. They still rely on a global, system-level installation of Python albeit they can refer to the proper version. So when we use Python 2.7 in a project, we’re pointing to an installation of Python 2.7 on the computer itself, not actually within the virtual environment.

### Also we can’t run a production database or other services within virtual environments so compared to Docker containers they are far more limited.

## Why do we need Docker?

- Faster development process
- Handy application encapsulation
- The same behaviour on local machine / dev / staging / production servers
- Easy and clear monitoring
- Easy to scale

## Library Website and API
### Django REST Framework works alongside the Django web framework to create web APIs. We cannot build a web API with only Django Rest Framework; it always must be added to a project after Django itself has been installed and configured.

### Django and DRF( Django Rest Framework ) are different in the way they are being used. If you want to create a web application django will be helpful for that and if you want to create APIs only then DRF can be useful.

### Once you install the Django REST framework package, add it to the INSTALLED_APPS list variable in your Django project's settings.py file with the name rest_framework. Once this is done, you can start working with the Django REST framework.






