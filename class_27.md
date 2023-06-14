# Class 27

**Date Due:** June 13, 2023, 6:30 p.m.

## Reading

- [_Using Models_](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models)
- [_Django Admin_](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Admin_site)

## Reading Questions

### Explain the purpose and basic structure of Django models. How do they help in creating and managing database schema in a Django application?

Django models are essentially Python classes that represent database tables. They identify the types of data used, their characteristics,
field types, default values, and other similar characteristics that let your application interact with the stored data.

### Describe the primary features and functionality of the Django Admin interface. How can it be customized to suit the specific needs of a project?

The Django Admin interface allows you to manage the data that is going to be used. It includes the basic CRUD operations, user permissions,
various views, inline editing, and relationship management. It can be customized with list views and detail views, making it easier to examine
and interact with the ddata.

### Briefly outline the key components and workflow of a Django application, as discussed in the Beginner’s Guide to Django. How do these components interact with each other to create a functional web application?

- Models: Control the data structure and behavior of the application
- Database: The tables that store the application's data
- URLs: Determine how specific URLs map to various parts of the application
- Views: Handle the logic of the incoming and outgoing requests
- Templates: Define the actual structure and layout of the application into which the data will flow
