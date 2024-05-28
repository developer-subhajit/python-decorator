# `classmethod`

> This decorator is used to define a method that's bound to the class and not the instance. It can be called on the class itself, and it has access to the class state that can modify class variables.

```python
class MyClass:
    class_variable = 0

    @classmethod
    def increment_class_variable(cls):
        cls.class_variable += 1

MyClass.increment_class_variable()
print(MyClass.class_variable)  # Outputs: 1
```

In this example, `increment_class_variable` is a class method that increments the `class_variable
` of `MyClass`. It's called on the class itself, and it modifies the class state.
