# Quick Start

## Install

```bash
pip install fynor
```

## Basic Usage

```python
from fynor import Fynor

app = Fynor()

@app.route("/")
def home(req, resp):
    resp.text = "Hello, this is a home page."

@app.route("/about")
def about_page(req, resp):
    resp.text = "Hello, this is an about page."
```
