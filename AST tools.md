## AST Tools of Python & JavaScript

### Python

#### code to AST

1. `ast` : module in Python library

official documentation: https://docs.python.org/3/library/ast.html

a detailed documentation: https://greentreesnakes.readthedocs.io/en/latest/



2. `typed-ast` : a third-party package

> typed_ast is a Python 3 package that provides a Python 2.7 and Python 3
> parser similar to the standard ast library.  Unlike ast, the parsers in
> typed_ast include PEP 484 type comments and are independent of the version of
> Python under which they are run.  The typed_ast parsers produce the standard
> Python AST (plus type comments), and are both fast and correct, as they are
> based on the CPython 2.7 and 3.6 parsers.

pypi: https://pypi.org/project/typed-ast/

github project:  https://github.com/python/typed_ast



3. PathMiner: extract path-context information as input of code2vec

github project: https://github.com/vovak/astminer

example of Python code: https://github.com/vovak/astminer/tree/master/src/main/kotlin/astminer/examples/pyExample



#### AST to code

1. `astor` : a third-party package, features include:
   + operations on AST, similar to `ast`
   + convert AST to code in Python

pypI: https://pypi.org/project/astor/
documentation: https://astor.readthedocs.io
github project: https://github.com/berkerpeksag/astor



#### Visualize AST

1. `python-ast-explorer` : a tool to visualize AST of Python code

github project: https://github.com/maligree/python-ast-explorer/

website: https://python-ast-explorer.com/



2. `show_ast`:  an IPython notebook plugin for visualizing AST of Python code

github project: https://github.com/hchasestevens/show_ast



3. `instaviz` : a third-party package for visualizing AST of Python code in Web Browser

pypi: https://pypi.org/project/instaviz/

github project: https://github.com/tonybaloney/instaviz



### JavaScript

1. slimit

parse raw javascript code into AST

pypi: https://pypi.org/project/slimit/

homepage: https://slimit.readthedocs.io/en/latest/

