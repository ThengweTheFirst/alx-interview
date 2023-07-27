# 0x04. UTF-8 Validation

## Algorithm
The project "0x04. UTF-8 Validation" focuses on implementing a Python method that determines if a given data set represents a valid UTF-8 encoding. The data set consists of a list of integers, where each integer represents 1 byte of data (8 least significant bits of each integer). The method should return `True` if the data is a valid UTF-8 encoding, and `False` otherwise.

## Resources
Read or watch:
- [UTF-8](https://en.wikipedia.org/wiki/UTF-8)
- [Characters, Symbols, and the Unicode Miracle](https://www.youtube.com/watch?v=MijmeoH9LT4)

## Requirements
- Allowed editors: vi, vim, emacs
- All files will be interpreted/compiled on Ubuntu 14.04 LTS using python3 (version 3.4.3)
- All files should end with a new line
- The first line of all files should be exactly `#!/usr/bin/python3`
- A README.md file, at the root of the folder of the project, is mandatory
- Code should use the PEP 8 style (version 1.7.x)
- All files must be executable

## Tasks
### 0. UTF-8 Validation
Write a method that determines if a given data set represents a valid UTF-8 encoding.

**Prototype:** `def validUTF8(data) -> bool`
**Return:** `True` if data is a valid UTF-8 encoding, else return `False`

A character in UTF-8 can be 1 to 4 bytes long.
The data set can contain multiple characters.
The data will be represented by a list of integers, where each integer represents 1 byte of data (8 least significant bits of each integer).

### Example
```python
data = [65]
print(validUTF8(data))  # Output: True

data = [80, 121, 116, 104, 111, 110, 32, 105, 115, 32, 99, 111, 111, 108, 33]
print(validUTF8(data))  # Output: True

data = [229, 65, 127, 256]
print(validUTF8(data))  # Output: False
```

## Repository Information
- GitHub repository: alx-interview
- Directory: 0x04-utf8_validation
- File: 0-validate_utf8.py

---

*This project is part of the interview preparation projects for Holberton School.*
