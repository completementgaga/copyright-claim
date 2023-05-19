# npGUI

This very simple python package allows to add or remove copyright/license claims at
the beginning of your  source files (single file use or whole folder use, the
files being filtered based on their extensions).

 Yes it has only two functions !


Yet, it also defines a terminal command that allows to call the add and remove functions.



## Installation
This package can be installed with pip as follows.

```
$ pip install copyright-claim
```

Most likely, you need not install this package in a virtual environment,
since its only dependencies are packages which are provided
in the standard library at least since version 3.7 of Python. 



## Documentation

A detailed documentation of this package is available on 
[GitHub Pages](https://completementgaga.github.io/copyright-claim/) --- as a website.

It is also available in pdf format
[here](https://github.com/completementgaga/npGUI/blob/master/sphinx/build/latex/npgui.pdf).

For the command line version, if you used pip to install the package,

you can run 
```
$ copyright-claim -h
```
in your terminal and observe
```
usage: copyright_claim [-h] [--claim_path CLAIM_PATH] [-r] [--extension EXTENSION] [--comment_symbol COMMENT_SYMBOL] {add,remove} project_path

Adds and removes copyright claims at the beginning of text files.

positional arguments:
  {add,remove}          Choose "add" if you want to add the claim, "remove" if you want to remove it.
  project_path          The path to the file or directory to be treated.

options:
  -h, --help            show this help message and exit
  --claim_path CLAIM_PATH, -c CLAIM_PATH
                        In case the add option is used, this argument is necessary. Useless otherwise.
  -r                    This flag must be used when treating a directory is desired. In this case all the file within the directory and its subdirectories will be affected, provided they have the chosen extension.
  --extension EXTENSION, -e EXTENSION
                        The extension that characterizes the file(s) to be treated. Defaults to ".py". When processing a single file, this argument is ignored.
  --comment_symbol COMMENT_SYMBOL
                        The string to be used to comment out the lines of the claim block. Defaults to '# '.
```



## Further developments of the project

Feel free to open the discussion through issues and pull requests on the [GitHub repository](https://github.com/completementgaga/copyright-claim).

Feedback is also welcome by e-mail or by giving the project a star.














