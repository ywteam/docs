# sdk:term

Execute a command with given arguments

## Overview

Executes a command with provided arguments after verifying the command exists.
If command is not found, logs an error and returns failure.

## Index

* [sdk:term](#sdkterm)

## term

### sdk:term

Executes a command with provided arguments after verifying the command exists.
If command is not found, logs an error and returns failure.

#### Example

```bash
sdk:term ls -la 7>&1 | sdk:log:stdin "info" "term.colors"
sdk:term echo "Hello World" 7>&1 | sdk:log:stdin "info" "term.colors"
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

* [sdk:log](#sdklog)

