# Class 28

## Due Date: Jun 17, 2023, 9 a.m. PDT

## Reading

- [_Django Forms_](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms)

## Bookmark and Review

- [_Django Templates_](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Home_page)
- [_Django Views_](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Generic_views)

## Reading Questions

### How do Django Forms facilitate user input handling, and what are some key components of creating a form using the Django framework?

Django Forms facilitate user handling by taking care of data validation, rendering the form itself,
providing cross-site request forgery protection, and dealing with all the particulars of form
submission. Some of the key components of creating a form include the Forms class, field types, and creating the views that are required to perform the CRUD operations that will arise from the submission of these
forms.

### Explain the purpose of Django Templates in web development and describe how template inheritance can be utilized to improve code reusability and maintainability

Templates essentially form the basic structure of how the pages will be rendered. It is in these templates
that you indicate where certain fields or other types of data will be placed and often contain code, for
example, to iterate through all objects in a collection and render separate components based on those results.
Template inheritance allows the developer to create a base template that may contain pieces of the final
page that are shared by all pages within the site. The user can simply develop smaller, page-specific templates
that handle those specific functions while inheriting the base template, rather than rewriting the base
template code for each new template.

### Describe the function of Django Views in handling HTTP requests, and outline the differences between function-based views and class-based views

Views are responsible for handling incoming HTTP requests, perfoming actions (such as CRUD operations),
and then returning the appropriate response. They determine how to reply and what to display based
on the requested URL.

Function-based views acutally take a HTTP request as an argument (like a callback function) and return
the HTTP response. Class-based views are a more object-oriented approach to handling requests, and they
come with built-in functions for handling specific types of requests. In general, function-based views
are more easily customizable, while class-based views tend to come with more "in-the-box" functionality.
