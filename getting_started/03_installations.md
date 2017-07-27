## Installations

 Most Mac and linux systems have python pre installed.
 In this course we will be using **Python3**. This was a major version update from **Python2** with new features and syntax changes. Python3 is also the future of Python and is best we learn how to use them.

 ### Linux Installation

 #### Step 1: Check if Python3.6 is Installed.

 Open the terminal   Press  _ctrl+alt+t_   and type in `python3.6`.

 ```bash
 $ python3.6
 python3.6: command not found
 ```
 If it **does not** give that error it means you have `python3.6` Installed and you can move on with Python Basics.

 #### Step 2: Install Python3.6.

 On the terminal copy the following individual commands  on your console

 ```bash
$ sudo add-apt-repository ppa:jonathonf/python-3.6
$ sudo apt-get update
$ sudo apt-get install python3.6
 ```
 When prompted put in your password and leave the commands to run.

 #### Step 3 : Confirm Installation.

 On the terminal type in `python3.6` and we should have an output similar to this.
 ```bash
 $ python3.6

 Python 3.6.0 (default, Nov 17 2016, 17:05:23)
[GCC 5.4.0 20160609] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>>
 ```
To get out of this interface use the `exit()` function.

 ```bash
 $ python3.6

 Python 3.6.0 (default, Nov 17 2016, 17:05:23)
[GCC 5.4.0 20160609] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> exit()

$

 ```

 ### Mac Installation

 #### Step 1: Check if Python3.6 is Installed.

 Open the terminal   Press  _ctrl+alt+t_   and type in `python3.6`.

 ```bash
 $ python3.6
 python3.6: command not found
 ```
 If it **does not** give that error it means you have `python3.6` Installed and you can move on with Python Basics.

 #### Step 2: Download Python3 latest release.

 Go to https://www.python.org/downloads/ and download the latest release of Python3

 #### Step 3: Install Downloaded File.

 Install the downloaded file by following the installation instructions that follow.

  #### Step 4 : Confirm Installation.

 On the terminal type in `python3.6` and we should have an output similar to this.
```bash
Python 3.6.0 (default, Nov 17 2016, 17:05:23)
Type "help", "copyright", "credits" or "license" for more information.
>>>
```
To get out of this interface use the `exit()` function.

 ```bash
 $ python3.6

 Python 3.6.0 (default, Nov 17 2016, 17:05:23)
[GCC 5.4.0 20160609] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> exit()

$

 ```

 ### Installing Third party modules
 Other than the built in standard library of modules,Python developers have created their own modules to further extend python's functionality.

 The best way to install these python modules is to use pythons **pip** tool.

 These downloads python modules from https://pypi.python.org/ which is the pythons package index. A form of free app store for python modules

 #### Installing pip3
 Pip comes installed with python on Mac when you install python3 but for linux run this command

 ```bash
 $ sudo apt-get install python3-pip

 ```

Once Installations are done, we can move on and start learning some Python

---
### Time for [Feedback](https://goo.gl/forms/eVTveYUjyeQUTZDg2)
