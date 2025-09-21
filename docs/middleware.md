# Middleware

```python
from fynor.middleware import Middleware

class SimpleCustomMiddleware(Middleware):
    def process_request(self, req):
        print("Before dispatch", req.url)

    def process_response(self, req, res):
        print("After dispatch", req.url)

app.add_middleware(SimpleCustomMiddleware)
```
