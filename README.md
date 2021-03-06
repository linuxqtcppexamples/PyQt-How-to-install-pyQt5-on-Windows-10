# PyQt-How-to-install-pyQt5-on-Windows-10
How to install pyQt5 on Windows 10
How to install pyQt5 on Windows 10

Step1:

Download and install latest python exe from https://www.python.org/downloads/

Step2:

Update pip version if any update available using below command

python -m pip install --upgrade pip

Example:
C:\Users\<username>\AppData\Local\Programs\Python\Python38-32\Scripts>python -m pip install --upgrade pip

Step3:

Install PyQt5 using below command - recommended methoed
C:\Users\<username>\AppData\Local\Programs\Python\Python38-32\Scripts>pip.exe install pyQt5

(or)

Download pyQt5 whl(wheel) file from https://pypi.org/project/PyQt5
Install whl(wheel) file using below command

C:\Users\<username>\AppData\Local\Programs\Python\Python38-32\Scripts>pip.exe install D:\Softwares\PyQt5-5.14.1-5.14.0-cp35.cp36.cp37.cp38-none-win_amd64.whl


Python (programming language):(https://en.wikipedia.org/wiki/Python_(programming_language))
------------------------------
Python is an interpreted, high-level, general-purpose programming language. Created by Guido van Rossum and first released in 1991, 
Python's design philosophy emphasizes code readability with its notable use of significant whitespace. Its language constructs and 
object-oriented approach aim to help programmers write clear, logical code for small and large-scale projects.

Python is dynamically typed and garbage-collected. It supports multiple programming paradigms, including procedural, object-oriented, 
and functional programming. Python is often described as a "batteries included" language due to its comprehensive standard library.

Python was conceived in the late 1980s as a successor to the ABC language. Python 2.0, released in 2000, introduced features like list 
comprehensions and a garbage collection system capable of collecting reference cycles. Python 3.0, released in 2008, was a major revision of the language that is not completely backward-compatible, and much Python 2 code does not run unmodified on Python 3.

The Python 2 language, i.e. Python 2.7.x, was officially discontinued on January 1, 2020 (first planned for 2015) after which security 
patches and other improvements will not be released for it. With Python 2's end-of-life, only Python 3.5.x[32] and later are supported.

Python interpreters are available for many operating systems. A global community of programmers develops and maintains CPython, an open
source reference implementation. A non-profit organization, the Python Software Foundation, manages and directs resources for Python and CPython development

pip (package manager):
----------------------
pip is a de facto standard package-management system used to install and manage software packages written in Python. Many packages 
can be found in the default source for packages and their dependencies — Python Package Index (PyPI).

Most distributions of Python come with pip preinstalled. Python 2.7.9 and later (on the python2 series), and Python 3.4 and later 
include pip (pip3 for Python 3) by default.

pip is a recursive acronym for "Pip Installs Packages".

Command-line interface

An output of pip install virtualenv
One major advantage of pip is the ease of its command-line interface, which makes installing Python software packages as easy as issuing
a command:

pip install some-package-name

Users can also easily remove the package:

pip uninstall some-package-name

Most importantly pip has a feature to manage full lists of packages and corresponding version numbers, possible through a "requirements" file.[5] This permits the efficient re-creation of an entire group of packages in a separate environment (e.g. another computer) or virtual environment. This can be achieved with a properly formatted file and the following command[8], where requirements.txt is the name of the file:

pip install -r requirements.txt

Install some package for a specific version python, where ${version} is replaced for 2, 3, 3.4, etc.:

pip${version} install some-package-name

pip list -> it will display install packages
pip show <installed package name> -> it will inoformation about installed packages like installation path


PyQt:(https://en.wikipedia.org/wiki/PyQt)
-----
PyQt is a Python binding of the cross-platform GUI toolkit Qt, implemented as a Python plug-in. PyQt is free software developed by the
British firm Riverbank Computing. It is available under similar terms to Qt versions older than 4.5; this means a variety of licenses 
including GNU General Public License (GPL) and commercial license, but not the GNU Lesser General Public License (LGPL). 
PyQt supports Microsoft Windows as well as various flavours of UNIX, including Linux and MacOS (or Darwin).

PyQt implements around 440 classes and over 6,000 functions and methods including:

a substantial set of GUI widgets
classes for accessing SQL databases (ODBC, MySQL, PostgreSQL, Oracle, SQLite)
QScintilla, Scintilla-based rich text editor widget
data aware widgets that are automatically populated from a database
an XML parser
SVG support
classes for embedding ActiveX controls on Windows (only in commercial version)
To automatically generate these bindings, Phil Thompson developed the tool SIP, which is also used in other projects.

In August 2009, Nokia, the then owners of the Qt toolkit, released PySide, providing similar functionality, but under the LGPL,
after failing to reach an agreement with Riverbank Computing to change its licensing terms to include LGPL as an alternative license.

What is SIP?
------------
One of the features of Python that makes it so powerful is the ability to take existing libraries, written in C or C++, and make them available as Python extension modules. Such extension modules are often called bindings for the library.

SIP is a collection of tools that makes it very easy to create Python bindings for C and C++ libraries. It was originally developed in 1998 to create PyQt, the Python bindings for the Qt toolkit, but can be used to create bindings for any C or C++ library. For example it is also used to generate wxPython, the Python bindings for wxWidgets.

SIP comprises a set of build tools and a sip module. The build tools process a set of specification files and generates C or C++ code which is then compiled to create the bindings extension module. Several extension modules may be installed in the same Python package. Extension modules can be built so that they are are independent of the version of Python being used. In other words a wheel created from them can be installed with any version of Python starting with v3.5.

The specification files contain a description of the interface of the C or C++ library, i.e. the classes, methods, functions and variables. The format of a specification file is almost identical to a C or C++ header file, so much so that the easiest way of creating a specification file is to edit a copy of the corresponding header file.

The sip module provides support functions to the automatically generated code. The sip module is installed as part of the same Python package as the generated extension modules. Unlike the extension modules the sip module is specific to a particular version of Python (e.g. v3.5, v3.6, v3.7, v3.8).

SIP makes it easy to exploit existing C or C++ libraries in a productive interpretive programming environment. SIP also makes it easy to take a Python application (maybe a prototype) and selectively implement parts of the application (maybe for performance reasons) in C or C++.
