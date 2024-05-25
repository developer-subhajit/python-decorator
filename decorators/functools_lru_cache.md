# `functools.lru_cache`

> This decorator provides a least-recently-used (LRU) cache for function results. It can significantly speed up repeated calls with the same arguments by caching the results.

```python
import functools

@functools.lru_cache(maxsize=32)
def fibonacci(n):
    if n < 2:
            return n
    return fibonacci(n-1) + fibonacci(n-2)

print(fibonacci(100))  # Computes and caches results
print(fibonacci.cache_info())  # Outputs cache statistics
```
