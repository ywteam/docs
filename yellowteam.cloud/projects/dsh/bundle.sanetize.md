# bundle.sanetize.sh

Sanitizes shell script file by removing empty lines, comments, and specific replacements

## Overview

This function processes a shell script file by:
- Removing empty lines
- Removing comment lines
- Removing carriage returns
- Replacing 'exit' commands with 'return'
- Replacing version string with branch/commit format

## Index

* [dsh:bundle:sanetize](#dshbundlesanetize)

## Bundle

### dsh:bundle:sanetize

This function processes a shell script file by:
- Removing empty lines
- Removing comment lines
- Removing carriage returns
- Replacing 'exit' commands with 'return'
- Replacing version string with branch/commit format

#### Example

```bash
dsh:bundle:sanetize "/path/to/script.sh"
```

#### Arguments

* **$1** (Path): to the shell script file to sanitize

#### Exit codes

* **0**: If script file was successfully sanitized 
* **1**: If script file path is empty or file doesn't exist

#### Output on stdout

* Outputs sanitized script content to stdout

#### See also

* [sed](#sed)

