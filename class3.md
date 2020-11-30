# summery
## Reading and Writing Files in Python
![image](https://1.bp.blogspot.com/-8rb2wm5S3JM/Xxb6qgwJ9II/AAAAAAAAExs/Awbdyv36DasysU6u5mgVYdqPS3lofRXgACNcBGAsYHQ/w1200-h630-p-k-no-nu/Webp.net-compress-image%2B%25285%2529.jpg)
##### One of the most common tasks that you can do with Python is reading and writing files. Whether it’s writing to a simple text file, reading a complicated server log, or even analyzing raw byte data, all of these situations require reading or writing a file.
### first let's know ***what is the file***
##### file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable.
#### the file composed of three main part:
1. Header: metadata about the contents of the file (file name, size, type, and so on)
2. Data: contents of the file as written by the creator or editor
3. End of file (EOF): special character that indicates the end of the file
### now let's move to the File Paths
#### When you access a file on an operating system, a file path is required. The file path is a string that represents the location of a file. It’s broken up into three major parts:
1. Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)
2. File Name: the actual name of the file
3. Extension: the end of the file path pre-pended with a period (.) used to indicate the file type
#### take this example to understand
`` /
│
├── path/
|   │
│   ├── to/
│   │   └── cats.gif
│   │
│   └── dog_breeds.txt
|
└── animals.csv ``
### what about Line Endings
#### One problem often encountered when working with file data is the representation of a new line or line ending. also Windows uses the CR+LF characters to indicate a new line
#### okay it's confiuse :) Here’s a quick example. Let’s say that we examine the file dog_breeds.txt that was created on a Windows system:
`` Pug\r\n 
Jack Russell Terrier\r\n
English Springer Spaniel\r\n
German Shepherd\r\n
Staffordshire Bull Terrier\r\n
Cavalier King Charles Spaniel\r\n
Golden Retriever\r\n
West Highland White Terrier\r\n
Boxer\r\n
Border Terrier\r\n `` 
#### This same output will be interpreted on a Unix device differently:
`` Pug\r
\n
Jack Russell Terrier\r
\n
English Springer Spaniel\r
\n
German Shepherd\r
\n
Staffordshire Bull Terrier\r
\n
Cavalier King Charles Spaniel\r
\n
Golden Retriever\r
\n
West Highland White Terrier\r
\n
Boxer\r
\n
Border Terrier\r
\n``
#### Pug\r
\n
Jack Russell Terrier\r
\n
English Springer Spaniel\r
\n
German Shepherd\r
\n
Staffordshire Bull Terrier\r
\n
Cavalier King Charles Spaniel\r
\n
Golden Retriever\r
\n
West Highland White Terrier\r
\n
Boxer\r
\n
Border Terrier\r
\n ``
#### This can make iterating over each line problematic, and you may need to account for situations like this.
## Opening and Closing a File in Python
#### When you want to work with a file, 1. the first thing to do is to open it. This is done by invoking the `` open() ``
#### ex : `file = open('dog_breeds.txt') `
2. After you open a file, the next thing to learn is how to close it.
#### ex :  `` reader.close() `` or `` with open('dog_breeds.txt') as reader: `` 
3. Once you’ve opened up a file, you’ll want to read or write to the file
4. reading a file. There are multiple methods that can be called on a file object to help you out
#### ex : `` .read(size=-1) `` and `` .readline(size=-1) `` and `` .readlines() ``
5. Now let’s dive into writing files As with reading files, file objects have multiple methods that are useful for writing to a file:
#### ex : ``.write(string) `` and `` writelines(seq) ``
### for more information see this website [linke](https://realpython.com/read-write-files-python/)
## now let's move to our another topic which is Python Exceptions
![image](https://i.morioh.com/2019/12/23/e6f4b16f4dd2.jpg)
### Syntax Errors
#### there are multipal type of syntax error 
- SyntaxError: invalid syntax
- ZeroDivisionError: integer division or modulo by zero
### What is Exception?
#### An exception is an event, which occurs during the execution of a program that disrupts the normal flow of the program’s instructions. In general, when a Python script encounters a situation that it cannot cope with, it raises an exception. An exception is a Python object that represents an error.

#### When a Python script raises an exception, it must either handle the exception immediately otherwise it terminates and quits

### Raising an Exceptions
#### You can raise exceptions in several ways by using the raise statement. The general syntax for the raise statement is as follows.

#### Syntax raise [Exception [, args [, traceback]]]

#### Here, Exception is the type of exception (for example, NameError) and argument is a value for the exception argument. The argument is optional; if not supplied, the exception argument is None.






   






