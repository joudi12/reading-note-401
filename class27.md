# summery 
## Django Models
![image](https://pythondevs.org/wp-content/uploads/2020/04/why_django_is_the_best_web_framework_for_your_project_2_image_1.png)
### A model is the single, definitive source of information about your data. It contains the essential fields and behaviors of the data you’re storing. Generally, each model maps to a single database table.
### The basics:

- Each model is a Python class that subclasses django.db.models.Model.
- Each attribute of the model represents a database field.
- With all of this, Django gives you an automatically-generated database-access API; see Making queries.

## the difference between SQL and  Django models in  ways of writing data
![image2](https://djangobook.com/wp-content/uploads/Django_ORM_600.png)

### In Django, the model is the object mapped to the database. When you create a model, Django executes SQL to create a corresponding table in the database without you having to write a single line of SQL. Django prefixes the table name with the name of your Django application. The model also links related information in the database.

![image3](https://djangobook.com/wp-content/uploads/model_table1_600.png)


## Designing the LocalLibrary models
### When designing your models it makes sense to have separate models for every "object" (a group of related information).
### Once we've decided on our models and field, we need to think about the relationships. Django allows you to define relationships that are one to one (OneToOneField), one to many (ForeignKey) and many to many (ManyToManyField).
## Creating a Model
### Models are usually defined in an application's models.py file. They are implemented as subclasses of django.db.models.Model, and can include fields, methods and metadata.
```
from django.db import models

class MyModelName(models.Model):
    """A typical class defining a model, derived from the Model class."""

    # Fields
    my_field_name = models.CharField(max_length=20, help_text='Enter field documentation')
    ...

    # Metadata
    class Meta:
        ordering = ['-my_field_name']

    # Methods
    def get_absolute_url(self):
        """Returns the url to access a particular instance of MyModelName."""
        return reverse('model-detail-view', args=[str(self.id)])

    def __str__(self):
        """String for representing the MyModelName object (in Admin site etc.)."""
        return self.my_field_name
```

## Metadata
### You can declare model-level metadata for your Model by declaring class Meta, as shown.
```
class Meta:
    ordering = ['-my_field_name']
```    
