# [Django Forms](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms)

These technical documents dont do me any good at this stage. So instead of reading this article, I watched [this](https://www.youtube.com/watch?v=vM9mcWr1RMg) video.

functionally the same as a html form. But with python! how its done with Django:

example form - Asume the code below is in some .html file that needs a form
```python
{% block content %}
Create Form
<form method='post' action='/create/'>
	{% csrf_token %}
	{{form.as_p}} # as_p will move the next lines down, like a block level elem
	<button type='submit', name='save'>Save form</button>
</form>
{% endblock %}

```

Now in a forms.py file
```python
from django import forms

class Form(froms.form): # inheiret the default form class
	# these are the same as the fields in the DB
	name = froms.CharField(label="Name", max_length=256) # the label her denotes the forms name
	
	
```

