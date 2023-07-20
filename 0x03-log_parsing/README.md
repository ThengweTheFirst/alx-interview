## Log Parsing

This project aims to create a script called `0-stats.py` that reads input from stdin line by line and computes metrics based on the log data provided.

### Requirements

- Allowed editors: vi, vim, emacs
- All your files will be interpreted/compiled on Ubuntu 14.04 LTS using Python 3 (version 3.4.3)
- All your files should end with a new line
- The first line of all your files should be exactly `#!/usr/bin/python3`
- A `README.md` file, at the root of the folder of the project, is mandatory## Log Parsing

This project aims to create a script called `0-stats.py` that reads input from stdin line by line and computes metrics based on the log data provided.

### Requirements

- Allowed editors: vi, vim, emacs
- All your files will be interpreted/compiled on Ubuntu 14.04 LTS using Python 3 (version 3.4.3)
- All your files should end with a new line
- The first line of all your files should be exactly `#!/usr/bin/python3`
- A `README.md` file, at the root of the folder of the project, is mandatory
- Your code should follow the PEP 8 style (version 1.7.x)
- All your files must be executable
- The length of your files will be tested using `wc`

### Tasks

#### Task 0: Log parsing

Write a script `0-stats.py` that reads stdin line by line and computes metrics based on the log data. The input format should be as follows:

```
<IP Address> - [<date>] "GET /projects/260 HTTP/1.1" <status code> <file size>
```

If the format is not as specified above, the line should be skipped.

After every 10 lines and/or a keyboard interruption (CTRL + C), the script should print the following statistics from the beginning:

1. Total file size: File size: `<total size>` (where `<total size>` is the sum of all previous `<file size>` values).
2. Number of lines by status code: The script should count and print the occurrences of the following possible status codes: 200, 301, 400, 401, 403, 404, 405, and 500. If a status code doesn’t appear or is not an integer, don’t print anything for this status code. The status codes should be printed in ascending order.

**Sample Usage:**

```bash
$ ./0-generator.py | ./0-stats.py
File size: 5213
200: 2
401: 1
403: 2
404: 1
405: 1
500: 3
File size: 11320
200: 3
301: 2
400: 1
401: 2
403: 3
404: 4
405: 2
500: 3
File size: 16305
200: 3
301: 3
400: 4
401: 2
403: 5
404: 5
405: 4
500: 4
^CFile size: 17146
200: 4
301: 3
400: 4
401: 2
403: 6
404: 6
405: 4
500: 4
```

**Note:** The output might vary due to random values in the `0-generator.py` script.

