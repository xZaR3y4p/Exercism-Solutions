# Instructions append

## Exception messages

Sometimes it is necessary to [raise an exception](https://docs.python.org/3/tutorial/errors.html#raising-exceptions). When you do this, you should always include a **meaningful error message** to indicate what the source of the error is. This makes your code more readable and helps significantly with debugging. For situations where you know that the error source will be a certain type, you can choose to raise one of the [built in error types](https://docs.python.org/3/library/exceptions.html#base-classes), but should still include a meaningful message.

This particular exercise requires that you use the [raise statement](https://docs.python.org/3/reference/simple_stmts.html#the-raise-statement) to "throw" a `ValueError` if the `preorder` and `inorder` arguments are mis-matched length-wise, element-wise, or the elements are not unique. The tests will only pass if you both `raise` the `exception` and include a message with it.

To raise a `ValueError` with a message, write the message as an argument to the `exception` type:

```python
# if preorder and inorder are not the same length
raise ValueError("traversals must have the same length")

# if preorder and inorder do not share the same elements
raise ValueError("traversals must have the same elements")
    
# if element repeat (are not unique)    
raise ValueError("traversals must contain unique items")
```
