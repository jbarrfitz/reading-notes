# Class 17

**Date Due:** May 12, 9am PDT

## Reading

- [_Scrape a Dynamic Website with Python_](https://scrapingant.com/blog/scrape-dynamic-website-with-python)
- [_What is Web Scraping?_](https://en.wikipedia.org/wiki/Web_scraping)
- [_How to Scrape Websites without Getting Blocked_](https://www.scrapehero.com/how-to-prevent-getting-blacklisted-while-scraping/)

## Video

- [_Python Playwright Tutorial for Beginners_](https://www.youtube.com/watch?v=yp1o9biMMWU)

## Reading Questions

### What are the key differences between scraping static and dynamic websites?

Static websites render their content in such a way that you can view all of the data being requested
on the page load, whereas dynamic websites use internal JavaScript, AJAX, or other methods to dynamically
render the content.

### Explain at least three techniques or best practices that can be employed to avoid getting blocked while scraping websites

1. Making your requests through rotating proxies. By changing the IP address of where your requests are coming from, it makes it harder for websites to detect that they are being scraped.
2. Slowing down the crawling. Websites can reliably detect if they are being scraped if requests are coming in far faster than a human could ever make them.
3. Using Captcha solving services. There are tools out today designed to solve Catcha puzzles to help you get through these blocks.
4. Rotating user agents. Doing a lot of scraping using the same user agent is one way that websites can detect that they're being scraped by a bot.

### What is Playwright, and how does it assist in web scraping tasks? Provide an example of a use case where Playwright would be particularly beneficial

Playwright is an open source library that is designed to automate browser interactions that allows for both headless and headed automation, allowing
for both completed automated testing and for inspecting the actions to fine-tune the process.  This is particularly helpful in trying to scrape data
from, for example, social media sites. Playwright could automate the login process and simulate user actions such as searching for particular
trending topics on those social media platforms.

### Describe the purpose of using Xpath in web scraping, and provide an example of an Xpath expression to select a specific HTML element from a webpage

Xpath allows you to search for a specific element on a page, which helps in letting your automation know that you have reached the page you are
looking for. By looking for a specific element that is supposed to appear on that page, you can verifiy you're at the correct place. An example
Xpath expression to locate a specific element would be:

```python

//input[@id=username]

```
