# Class 16

**Date Due:** May 9, 6:30 pm PDT

## Reading

- [_What is Serverless Computing?_](https://www.ibm.com/cloud/learn/serverless)
- [_Seaborn Tutorial_](https://seaborn.pydata.org/tutorial.html)
- [_Bokeh Tutorial_](https://mybinder.org/v2/gh/bokeh/bokeh-notebooks/master?filepath=tutorial%2F00%20-%20Introduction%20and%20Setup.ipynb)

### Reading Questions

#### What are the key characteristics of serverless computing, and how does it differ from traditional server-based architectures?

Serverless applications use servers, but those servers are invisible to the developer. The cloud providers handles all of the services
in the background, including spinning up only the resources when necessary, and spinning them back down when they are no longer needed.
In this model, the services required are provided at runtime on an as-needed basis, which allows for much more efficient use of
resources.

### How can one get started with Vercel, and what are the main steps involved in deploying a serverless function using Vercel?

You can essentially just link your project via git using any supported platform, and Vercel will take care of providing the
services rqequired for running the application. Vercel will keep your project constantly updated whenever you commit changes. Vercel
automatically detects the services that are required. Additional setup will likely be required, such as setting up environment variables
and other development settings.

### What are APIs, and how can they be utilized in Python applications to access and manipulate data from external sources?

An API is an application programming interface, which essentially is the protocol by which a developer can communicate to an
outside system. Python provides the requests library for performing REST API calls. By providing the URL of the resource and
whatever credentials are required, you can request information from many sources using these calls.

### What is the Requests library in Python, and how can it be used to interact with APIs by sending HTTP requests? Can you provide an example of a basic GET request using the Requests library?

The Requests libary allows you to crerate RESTful API requests. the basic format of a get request is:

```python
response = requests.get("https://api.chucknorris.io/jokes/random")
print(response.json()["value"])
```
