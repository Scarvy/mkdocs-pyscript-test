# `mkdocs-pyscript` demo site

This page demos how PyScript can be used to make online documentation interactive. It is one of the demos created for the conference talk 'Making Your Documentation Interactive with PyScript' by Jeff Glass. See [more details on that talk](https://github.com/JeffersGlass/using-pyscript-in-documentation) or [the code for this site](https://github.com/JeffersGlass/mkdocs-pyscript-demo) on GitHub.


## The Datetime Module

The `datetime` module can be used to reference specific times, timespans, epochs, and calendar days.
Let's explore the relationship between the `datetime` and `timedelta` classes. If we create a new datetime:
```py
from datetime import datetime
d_1 = datetime(2023, 12, 1, 14, 30, 00)
print(d_1)
```
<br>

We can add a `timedelta` object to it to create another `datetime` object:

```py
from datetime import datetime, timedelta
d_1 = datetime(2023, 12, 1, 14, 30, 00)
delta = timedelta(days=90, hours=16, minutes=35)
d_2 = d_1 + delta
print(delta)
print(d_2)
```

Or we can subtract one `datetime` from another to create a `timedelta`:

```py
from datetime import datetime
d_3 = datetime(2023, 12, 14, 16, 30)
d_4 = datetime(2024, 5, 13, 11, 15)
print(d_3 - d_4)
```