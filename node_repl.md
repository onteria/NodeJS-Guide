Node.js comes complete with a REPL environment that can be used for quick prototyping of code. After installation of node, the node REPL can be started by issuing the `node` command at the terminal:

```
$ node
> 
```

From here various instructions can be evaluated. This includes evaluation of expressions, import of modules, assignment of variables, and execution of functions:

```
> 3+3
6
> var test = 3
> test
3
> var fs = require('fs');
> console.log("Hello World")
Hello World
```

Quitting the REPL at any time can be done by issuing the `.exit` or `process.exit()` command:

```
> .exit
$
> process.exit()
$
```

In the event of getting lost by a stray quote, or want to cancel the creation of a long amount of statements, the `.break` command can be used to get out:

```
> console.log("Hello World')
... .break
> 
```

It is also possible to start from a clean slate, without having to restart the REPL. This is done with the `.clear` command:

```
> var fs = require('fs');
> .clear
Clearing context...
> fs
ReferenceError: fs is not defined
```

These REPL specific commands can be displayed at any time with the `.help` command:

```
> .help
.break	Sometimes you get stuck, this gets you out
.clear	Break, and also clear the local context
.exit	Exit the repl
.help	Show repl options
```
