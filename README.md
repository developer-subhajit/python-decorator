# Python Decorators

A curated list of python decorator resources.

## Built-in python decorator

> -   [@functools.wraps](https://docs.python.org/3/library/functools.html#functools.wraps) : This decorator is used to preserve the metadata of the original function when it's wrapped by another function. It helps to keep the original function's name, docstring, and other attributes intact. Here is an [example](decorators/functools_wraps.md) of how to use.
> -   [@functools.cached_property](https://docs.python.org/3/library/functools.html#functools.cached_property) : This decorator transforms a method of a class into a property whose value is computed once and then cached as a normal attribute for the life of the instance. It's useful for expensive or I/O-bound operations that you want to cache. Here us an [example ](decorators/functools_cached_property.md) of how to use it.
> -   [@functools.lru_cache](https://docs.python.org/3/library/functools.html#functools.lru_cache) : This decorator provides a least-recently-used (LRU) cache for function results. It can significantly speed up repeated calls with the same arguments by caching the results.Here us an [example ](decorators/functools_lru_cache.md) of how to use it.
