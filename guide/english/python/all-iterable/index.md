---
title: Python All Iterable
---
`all()` is a built-in function in Python 3 (and Python 2 since version 2.5), to check if all items of an <a href='https://docs.python.org/3/glossary.html#term-iterable' target='_blank' rel='nofollow'>_iterable_</a> are `True`. It takes one argument, `iterable`.

## Argument

### iterable

The `iterable` argument is the collection whose entries are to be checked. It can be a `list`, `str`, `dict`, `tuple`, etc.

## Return Value

The return value is a Boolean. If and only if **all** entries of `iterable` are [truthy](https://guide.freecodecamp.org/python/truth-value-testing), it returns `True`. This function essentially performs a Boolean `AND` operation over all elements.

If even one of them is not truthy, it returns `False`. The following values are considered not truthy:
+ `None`
+ `False`
+ zero of any numeric type, for example, `0`, `0.0`, `0j`.
+ Any empty sequence, for example, `''`, `()`, `[]`.
+ Any empty mapping, for example, `{}`.


The `all()` operation is equivalent to (not internally implemented exactly like this)

    def all(iterable):
        for element in iterable:
            if not element:
                return False
        return True

## Code Sample

    print(all([])) #=> True  # Because an empty iterable has no non-truthy elements
    print(all([6, 7])) #=> True
    print(all([6, 7, None])) #=> False  # Because it has None
    print(all([6, 7, False])) #=> False  # Because it has False
    print(all([0, 6, 7])) #=> False  # Because it has zero
    print(all([9, 8, [1, 2]])) #=> True
    print(all([9, 8, ''])) #=> False  # Because it has '' 
    print(all([9, (), 8])) #=> False  # Because it has () 
    print(all([9, 8, []])) #=> False  # Because it has []
    print(all([9, 8, [1, 2, []]])) #=> True
    print(all([9, 8, {}])) #=> False  # Because it has {}
    print(all([9, 8, {'engine': 'Gcloud'}])) #=> True

🚀<a href='https://repl.it/@arverma/VacantVirtualPinkriverdolphin' target='_blank' rel='nofollow'>Run Code</a>

<a href='https://docs.python.org/3/library/functions.html#all' target='_blank' rel='nofollow'>Official Docs</a>

### Sources
1. <a href='https://docs.python.org/2/library/stdtypes.html#truth-value-testing' target='_blank'>Truth Value Testing. Accessed: October 20, 2018</a>
