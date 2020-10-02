---
title: Docstring
---
## Docstring

Docstring is a way for developers to communicate the purpose, parameters, requirements, and usage of a function in Python to other developers. It allows for ease of code maintenance and understanding.

Unlike conventional source code comments the docstring should describe what the
function does, not how.

A similar example to Docstring is @Javadoc in Java.

Docstring is written as a multi-line comment just after the declaration header in Python. There are 4 different parts to a docstring:

1. Type of input, and type of output
    * Input/output can be ```obj, list, bool, int, str, float```
2. Description of function
    * Brief, but thorough description of what your function does
3. Requirements 
    * This is read by a human, so it does not have to be code
4. Test cases (normally 2-3)

The general format is listed below.

## Format of Docstring

```python
def my_examplefunc(input_type1, input_type2):
    """
    Here is a description of my example function
    
    :param input_type1: Describe input_type1
    :type input_type1: Datatype of input_type1
    :return: Describe output
    :rtype: Datatype of output
    
    Test cases:
    >>> my_example_func([2, 3], "Hello World!")        
     [2, 3] "Hello World"
    """
    # Your code goes here, underneath the Docstring
```

Docstring is best understood with examples, so take a look at the below example program where the program outputs True if a number is less than 5, and False if a number is greater than 5.

## Example 1
```python
def is_less_than_five(some_number):
    """
    Returns True if the given number is less than 5, and False if it is greater than 5.
    
    :param some_number: Any real number not equal to 5
    :type some_number: float
    :return: True if the given number is less than 5 else False
    :rtype: bool
    
    Test cases:
    >>> is_less_than_five(4)
     True
    >>> is_less_than_five(6)
     False
    """
    # Your code goes here, underneath the Docstring
```

### Some useful links:
* PyCharm: https://www.jetbrains.com/help/pycharm/using-docstrings-to-specify-types.html#example
* Google: http://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html
* Numpy: http://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_numpy.html

Also, refer to some good old PEP commentary: https://www.python.org/dev/peps/pep-0257/
