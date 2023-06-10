# Class 26

**Date Due:** June 10, 9am PDT

## Reading

- [_Getting Started with Django_](https://www.djangoproject.com/start/)
- [_How Django Works Behind the Scenes_](https://wsvincent.com/how-django-works-behind-the-scenes/)
- [_What is Tailwind CSS_](https://blog.hubspot.com/website/what-is-tailwind-css)

## Bookmark and Review

- [_What is Django?_](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Introduction)
- [_First Django App Part 1_](https://docs.djangoproject.com/en/4.1/intro/tutorial01/)
- [_First Django App Part 2_](https://docs.djangoproject.com/en/4.1/intro/tutorial02/)
- [Tailwind CSS Django - Flowbite_](https://flowbite.com/docs/getting-started/django/)

## Reading Questions

### What are the key components of the Django framework, and how do they contribute to building a web application?

- Object-relational mapper: where you define your data model
- URLa and views: where you assign URL patterns to specific views for your website
- Templates: which definte the framework and structure of how your pages will be presented
- Forms: allowing for interactivity on the site
- Authentication: where you setup security, users, and permissions
- Admin: Provides an interface for content producers to manage the site
- Internationalization: Providing for translation of content for international users
- Security: Automatically provides protection against many commons threats such as SQL injection and remote code execution

### Explain the role of Django’s MTV (Model-View-Template) architecture and how it handles a typical web request-response cycle

- URLs: handles the mapping of the URL code that handles what view is being shown based on the URL
- Model: Defines the structure of the data and allows for record actions (like adding, modifying, deleting)
- View: Handles HTTP requests and responses
- Templates: Define the structure and layout on which the data will be displayed
  
#### Request-Response Cycle

- User sends a request to a specific URL
- URL dispatcher matches the URL to the corresponding view function
- The view function interacts with the model to retrieve or maniuplate the data
- The view function passes the data to the template, which renders the page

### What is the purpose of Tailwind CSS, and how does it differ from Bootstrap CSS?

Tailwind allows you to uses classes to write styling properties directly into the HTML. Unlike
Bootstrap, Tailwind does not provide fully-styled templates, but allows you to create them using
the classes to be able to tailor them much more fully. This allows you to keep the size of your
CSS files small and enables you to use custom styling without writing custom CSS.
