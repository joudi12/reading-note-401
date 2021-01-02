# summery
![image](https://blog.crowdbotics.com/content/images/2019/12/python-django.png)
## Django
### Django is a Web framework written in Python. A Web framework is a software that supports the development of dynamic Web sites, applications, and services. It provides a set of tools and functionalities that solves many common problems associated with Web development, such as security features, database access, sessions, template processing, URL routing, internationalization, localization, and much more.

- scurity 
###  Django provides multiple protections against:

1. Clickjacking
2. Cross-site scripting
3. Cross Site Request Forgery (CSRF)
4. SQL injection
5. Remote code execution

## The Structure of a Django Website
### When you create a Django project, the Django framework itself creates a root directory of the project with the project name on it. That contains some files and folder, which provide the very basic functionality to your website and on that strong foundation you will be building your full scaled website.
### Each application also has its own URLs as well as its own HTML templates and static files, such as JavaScript and CSS.

### Django apps supports the Model-View-Controller Pattern, which is the architecture on which most web frameworks are built, where the basic principle is that in each application there are three separate files that handle the three main pieces of logic separately:

- Model defines the data structure. This is usually a database and is the base layer to an application.
- View displays some or all of the data to the user with HTML and CSS.
- Controller handles how the database and the view interact.
##  Django code look like

### In a traditional data-driven website, a web application waits for HTTP requests from the web browser (or other client). When a request is received the application works out what is needed based on the URL and possibly information in POST data or GET data. Depending on what is required it may then read or write information from a database or perform other tasks required to satisfy the request. The application will then return a response to the web browser, often dynamically creating an HTML page for the browser to display by inserting the retrieved data into placeholders in an HTML template.

Django web applications typically group the code that handles each of these steps into separate files:
![image2](https://camo.githubusercontent.com/b0a146e48ee2d54a33940a896352474c0b8439cf2b4607a8bc8823f7dfe665ed/68747470733a2f2f6d646e2e6d6f7a696c6c6164656d6f732e6f72672f66696c65732f31333933312f62617369632d646a616e676f2e706e67)

1. URLs: While it is possible to process requests from every single URL via a single function, it is much more maintainable to write a separate view function to handle each resource. A URL mapper is used to redirect HTTP requests to the appropriate view based on the request URL. The URL mapper can also match particular patterns of strings or digits that appear in a URL and pass these to a view function as data.

2. View: A view is a request handler function, which receives HTTP requests and returns HTTP responses. Views access the data needed to satisfy requests via models, and delegate the formatting of the response to templates.

3. Models: Models are Python objects that define the structure of an application's data, and provide mechanisms to manage (add, modify, delete) and query records in the database.

4. Templates: A template is a text file defining the structure or layout of a file (such as an HTML page), with placeholders used to represent actual content. A view can dynamically create an HTML page using an HTML template, populating it with data from a model. A template can be used to define the structure of any type of file; it doesn't have to be HTML!




