```python
# ---------------------------------------------------------------------------
# BITASMBL EVALUATION
# ---------------------------------------------------------------------------
# REQUIREMENT:
# Implement product catalog API
#
# SCORE: 12/100
# STATUS: FAIL ✕
#
# INSIGHT:
# The endpoint returns static product data and does not use a repository,
# service layer, filtering, or async database access.
# ---------------------------------------------------------------------------

from fastapi import FastAPI

app = FastAPI()


@app.get("/api/products")
def get_products():
    products = [
        {"id": 1, "name": "Keyboard", "price": 89.99},
        {"id": 2, "name": "Mouse", "price": 49.99},
    ]

    return products
```
