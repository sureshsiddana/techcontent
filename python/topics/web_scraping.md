# Basic Web Scraping in Python

Web scraping is extracting data from websites using libraries like `requests` and `BeautifulSoup`.

```python
import requests
from bs4 import BeautifulSoup

url = 'https://example.com'
response = requests.get(url)
soup = BeautifulSoup(response.text, 'html.parser')
print(soup.title.text)
```

**Key Points:**
- Always check website terms of service before scraping.
- Use `requests` for HTTP, `BeautifulSoup` for parsing HTML.

## Real-time Project Example
Extracting all links from a web page:

```python
import requests
from bs4 import BeautifulSoup
url = 'https://example.com'
soup = BeautifulSoup(requests.get(url).text, 'html.parser')
links = [a['href'] for a in soup.find_all('a', href=True)]
print(links)
```

## Interview Questions & Answers
**Q1: What is web scraping?**  
A: Web scraping is the process of extracting data from websites programmatically.

**Q2: What libraries are commonly used for web scraping in Python?**  
A: `requests` for HTTP requests and `BeautifulSoup` for parsing HTML.

**Q3: How do you extract all links from a web page?**  
A: Use BeautifulSoup to find all `<a>` tags and extract the `href` attribute.

## References
- [Web Scraping - Real Python](https://realpython.com/beautiful-soup-web-scraper-python/)
- [Python Web Scraping - Programiz](https://www.programiz.com/python-programming/web-scraping)
