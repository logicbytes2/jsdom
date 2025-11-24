# JS-like DOM Wrapper in Python

A simple Python library that mimics JavaScript DOM manipulation using BeautifulSoup.

## Example Usage

```python
import pydom

html = "<html><body><nav id='nav'></nav></body></html>"
document = Document(html)

nav = document.getElementById("nav")
nav.innerHTML = "<h1>Hello World</h1>"

print(document.soup)

