# dsh:docs:template

Generate documentation template for shell functions

## Overview

Creates a standardized documentation template for shell functions following
shdoc format. The function generates basic documentation structure including
name, file path, section, and examples if provided.

## Index

* [dsh:docs:template](#dshdocstemplate)

## docs

### dsh:docs:template

Creates a standardized documentation template for shell functions following
shdoc format. The function generates basic documentation structure including
name, file path, section, and examples if provided.

#### Example

```bash
dsh:docs:template "myfunction.utils" --doc:brief="My utility function" --doc:example="myfunction.utils --help"
dsh:docs:template "test.core" --doc:example="test.core run" --doc:example="test.core clean"
```

#### Options

* --doc:*=* Documentation key-value pairs where * represents the documentation field

#### Arguments

* **$1** (string): The name of the function to document

#### Exit codes

* **0**: If successful, 1 otherwise
* **1**: If no name is provided

#### See also

* [dsh](#dsh)

