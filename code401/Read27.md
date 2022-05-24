# Django Models

### [Models](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models)

Funcitonaly a Django Model is simply a python object, they define the structure of stored datd including types and possibly max size, default values and more. 

You want to have separate models for every object.

>Once we've decided on our models and field, we need to think about the relationships. Django allows you to define relationships that are one to one (`OneToOneField`), one to many (`ForeignKey`) and many to many (`ManyToManyField`).
With that in mind, the UML association diagram below shows the models we'll define in this case (as boxes).
![LocalLibrary Model UML with fixed Author multiplicity inside the Book class](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models/local_library_model_uml.svg)

>The code fragment below shows a "typical" model, named `MyModelName`:

```python
from django.db import models
from django.urls import reverse

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
        """Returns the URL to access a particular instance of MyModelName."""
        return reverse('model-detail-view', args=[str(self.id)])

    def __str__(self):
        """String for representing the MyModelName object (in Admin site etc.)."""
        return self.my_field_name
```

All models can have methods, and all models should at least have a \__str__() method

# Django Admin 
### [Admin](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Admin_site)

A management style interface within django allowing you to create view update and delete records, Making it very easy to test models.

# Optional: Beginners guide to [Django](https://simpleisbetterthancomplex.com/series/2017/09/04/a-complete-beginners-guide-to-django-part-1.html)

