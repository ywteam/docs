# dsh:term

Execute a command with given arguments

## Overview

Executes a command with provided arguments after verifying the command exists.
If command is not found, logs an error and returns failure.

## Index

* [dsh:term](#dshterm)

## term

### dsh:term

Executes a command with provided arguments after verifying the command exists.
If command is not found, logs an error and returns failure.

#### Example

```bash
dsh:term ls -la 7>&1 | dsh:log:stdin "info" "term.colors"
dsh:term echo "Hello World" 7>&1 | dsh:log:stdin "info" "term.colors"
```

#### Options

* 1 Command to execute
* [2..n] Optional arguments to pass to the command

#### Exit codes

* **0**: Command executed successfully
* **1**: Command not found
* n Any exit code from executed command

#### Output on stderr

* Outputs error if command not found

#### See also

* [dsh:log](#dshlog)

