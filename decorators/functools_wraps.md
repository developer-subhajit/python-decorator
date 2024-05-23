# `functools.wraps`

> This decorator is used to preserve the metadata of the original function when it's wrapped by another function. It helps to keep the original function's name, docstring, and other attributes intact.

```python
import functools


def my_decorator(func):
	@functools.wraps(func)
	def wrapper(*args, **kwargs):
		print("Function is being called")
		return func(*args, **kwargs)

	return wrapper


@my_decorator
def say_hello():
	"""This function says hello"""
	print("Hello!")


say_hello()
print(say_hello.__name__) # Outputs: say_hello
print(say_hello.__doc__)  # Outputs: This function says hello

```
