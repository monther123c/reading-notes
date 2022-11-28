# Django Models
---
Using Models
Designing the LocalLibrary models
Once we've decided on our models and field, we need to think about the relationships. Django allows you to define relationships that are one to one (OneToOneField), one to many (ForeignKey) and many to many (ManyToManyField).
Model primer
Models are usually defined in an application's models.py file. They are implemented as subclasses of django.db.models.Model, and can include fields, methods and metadata.
Fields A model can have an arbitrary number of fields, of any type — each one represents a column of data that we want to store in one of our database tables. Each database record (row) will consist of one of each field value.

---

## How do you implement models in Django?
Prerequisites.
Step 1 — Create Django Application.
Step 2 — Add the Posts Model.
Step 3 — Update Settings.
Step 4 — Make Migrations.
Step 5 — Verify Database Schema.
---
### Is Django model a database?

A Django model is a table in your database.

==
#### Where are admin templates Django?
To view the default admin template you can access it in the django/contrib/admin/templates/admin folder.