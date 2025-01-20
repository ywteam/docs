# term.size.sh

Get terminal dimensions

## Overview

Determines the terminal size by attempting to use tput or stty commands.
Falls back to default values if neither command is available.

## Index

* [dsh:screen:size](#dshscreensize)

## term

### dsh:screen:size

Determines the terminal size by attempting to use tput or stty commands.
Falls back to default values if neither command is available.

#### Example

```bash
dsh:screen:size 7>&1 | dsh:log:stdin "info" "term.size"
# Output: 80 24
```

_Function has no arguments._

#### Variables set

* **DSH_SESSION["term.width"]** (Terminal): width in columns
* **DSH_SESSION["term.height"]** (Terminal): height in lines

#### Exit codes

* **0**: Successfully retrieved terminal dimensions
* **1**: Failed to get terminal dimensions

#### Output on stdout

* Space-separated terminal width and height values redirected to fd 7

#### See also

* [dsh:dep:exists Checks if required commands exist](#dshdepexists-checks-if-required-commands-exist)

