
# summery
![image](https://www.fellow-consulting.com/wp-content/uploads/2020/04/1_zW_Q1yUS4BJNVL6ibA6Q5Q.jpeg)


## Regular Expressions, often shortened as regex, are a sequence of characters used to check whether a pattern exists in a given text (string) or not
-  first of all you should install the regex 
`` import re ``
- there are alot of ruls for rugex you should to know it to be able to use regex 
![image2](https://twiki.org/p/pub/Codev/TWikiPresentation2013x03x07/regex-example-2.png)
## now let's talk about some method we can use it :
- match method : This function attempts to match RE pattern to string with optional flags.
``
re.match(pattern, string, flags=0)
``
- search method : One of the most important re methods that use regular expressions is sub. 
``
re.sub(pattern, repl, string, max=0)
``



# High-level file operations in Python (shutil)
![image3](https://i.ytimg.com/vi/hSTw7CAWRpo/mqdefault.jpg)
## what is shutil ???
### The shutil module includes high-level file operations such as copying and archiving.
### let's talk about some of it
1. rmtree() : This function removes files and subdirectories in the specified directory.


>>> shutil.rmtree('dir2')
>>> shutil.move('hello.py', 'newdir/')
'newdir/hello.py'
``



2. get_archive_formats():This function gives of all supported archive formats.

>>> shutil.get_archive_formats()
[('bztar', "bzip2'ed tar-file"), ('gztar', "gzip'ed tar-file"), ('tar', 'uncompressed tar file'), ('xztar', "xz'ed tar-file"), ('zip', 'ZIP file')]
``
3. which() :This function returns path to an executable.
>>> shutil.which('calc')
'C:\\WINDOWS\\system32\\calc.EXE'


### and there are more if you are interest join this [link](https://pymotw.com/3/shutil/)

---
