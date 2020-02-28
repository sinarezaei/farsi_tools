![alt text][pypi_version] ![alt text][licence_version]

# Farsi Tools: tools for processing Farsi (Persian) text

Tested with:
* Python 3.5+

Use the following command to install using pip:
```
pip install farsi-tools
```

## Usage example
### Converting digits

Use `replace_arabic_digits_with_farsi` method to replace arabic digits with farsi digits.
```python
from farsi_tools import replace_arabic_digits_with_farsi

replace_arabic_digits_with_farsi('٤')  # returns ۴
```

Use `replace_ascii_digits_with_farsi` method to replace ASCII digits with farsi digits.
```python
from farsi_tools import replace_ascii_digits_with_farsi

replace_ascii_digits_with_farsi('4')  # returns ۴
```

Use `replace_farsi_digits_with_ascii` method to replace farsi digits with ASCII digits.
```python
from farsi_tools import replace_farsi_digits_with_ascii

replace_farsi_digits_with_ascii('۴')  # returns 4
```

Use `replace_arabic_digits_with_ascii` method to replace farsi digits with ASCII digits.
```python
from farsi_tools import replace_arabic_digits_with_ascii

replace_arabic_digits_with_ascii('٤')  # returns 4
```


### Convert text to Farsi (Persian)
Use `standardize_persian_text` method to convert characters to standard persian form
```python
from farsi_tools import standardize_persian_text

standardize_persian_text('سلام خوبي؟ کمك ﻧميخواي؟') # returns "سلام خوبی؟ کمک نمیخوای؟"
```

### Get persian stop-words
Use `stopwords` method to retrieve list of persian stop-words
```python
from farsi_tools import stop_words

stop_words()
```


[pypi_version]: https://img.shields.io/pypi/v/pykson.svg "PYPI version"
[licence_version]: https://img.shields.io/badge/license-MIT%20v2-brightgreen.svg "MIT Licence"
