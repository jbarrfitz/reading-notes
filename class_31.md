# Reading Notes - Class 31

## Due Date: June 27, 2023, 6:30 p.m. PDT

## Reading

- [_Beginner's Guide to Docker_](https://wsvincent.com/beginners-guide-to-docker/)
- [_Django for APIs - Library Website](https://djangoforapis.com/library-website-and-api/)

## Bookmark and Review

- [_Beginner's Guide to Django REST Framework_](https://learndjango.com/tutorials/official-django-rest-framework-tutorial-beginners)

## Reading Questions

### What are the key components of a Docker container, and how do they help streamline the development and deployment of applications?

The primary components of a Docker container are the image, which is a lightweight package that contains
everything needed to run software; the Dockerfile, which is a text file that contains instructions for
building the image, and the container, which is the actual, running instance. They contain everything
needed to run an application on any computer, rather than having to install all the individual components
on each machine used.

### Describe the primary steps involved in building a library website using Django, including essential components like models, views, and templates

The primary steps include:

- Installing Django
- Adding a Django project
- Adding a Django app
- Registering the app with the project
- Registering the URLs to be used
- Creating a model, which is essentially how the data is going to be stored
- Creating views, which are the bridge between the model and any templates being used
- Creating the templates, which are the structure of the HTML files that will be rendered.

### Can you explain the primary differences between Django and Django REST framework?

Django is used primarily for website development, while the Django REST framework is used
for creating APIs. While templates are used in Django, DRF generally uses serialization
to format the output into JSON.
