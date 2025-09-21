# Handlers

## Function-based

```python
@app.route("/", allowed_methods=["get"])
def home(req, resp):
    resp.text = "Hello, this is a home page."
```

## Class-based

```python
@app.route("/{name:l}")
class GreetingHandler:
    def get(self, req, resp, name):
        resp.text = f"Hello, {name}"
```
