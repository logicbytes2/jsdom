How to use the Library
======================

1) Start by making sure pydom.py is in your working directory.
2) import the file into your python code ie.  import pydom
3) open the html code into your python code
4) Then simply use the methods as you would in javascript

** the library isn't an exact replica of javascript's functions but it feels very familiar

The code below is an example of how to use the library

import pydom
<code>
# Load HTML
with open("index.html", "r", encoding="utf-8") as f:
    raw = f.read()

document = pydom.Document(raw)

# Select an element in your html code
nav = document.getElementById("nav")

# Modify its innerHTML
nav.innerHTML = "<h1>Heavens above!</h1>"

# Save modified HTML
with open("index_modified.html", "w", encoding="utf-8") as f:
    f.write(str(document.soup))
</code>
