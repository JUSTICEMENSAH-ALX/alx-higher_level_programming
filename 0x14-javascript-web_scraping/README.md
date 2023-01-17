...................................................................................................................................................................................................................................................

Javascript - Web scraping

Learning Objectives

How to manipulate JSON data

How to use request and fetch API

How to read and write a file using fs module

Tasks

Readme

Write a script that reads and prints the content of a file.



The first argument is the file path

The content of the file must be read in utf-8

If an error occurred during the reading, print the error object

Solution: 0-readme.js



$ amonkeyprogrammer@ubuntu:~/0x14$ ./0-readme.js cisfun

C is super fun!

$ amonkeyprogrammer@ubuntu:~/0x14$ cat cisfun

C is super fun!

$ amonkeyprogrammer@ubuntu:~/0x14$ ./0-readme.js doesntexist

{ Error: ENOENT: no such file or directory, open 'doesntexist'

    at Error (native)

  errno: -2,

  code: 'ENOENT',

  syscall: 'open',

  path: 'doesntexist' }

$ amonkeyprogrammer@ubuntu:~/0x14$

Write me

Write a script that writes a string to a file.



The first argument is the file path

The second argument is the string to write

The content of the file must be written in utf-8

If an error occurred during while writing, print the error object

Solution: 1-writeme.js



$ amonkeyprogrammer@ubuntu:~/0x14$ ./1-writeme.js my_file.txt "Python is cool"

$ amonkeyprogrammer@ubuntu:~/0x14$ cat my_file.txt ; echo ""

Python is cool

$ amonkeyprogrammer@ubuntu:~/0x14$

Status code

Write a script that display the status code of a GET request.



The first argument is the URL to request (GET)

The status code must be printed like this: code: <status code>

You must use the module requests






........................................
