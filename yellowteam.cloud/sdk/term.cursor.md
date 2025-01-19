# term.cursor.sh

Control terminal cursor position and visibility

## Overview

A collection of functions to manipulate terminal cursor position and visibility

## Index

* [sdk:cursor](#sdkcursor)

## cursor

A collection of functions to manipulate terminal cursor position and visibility

### sdk:cursor

Provides commands to move cursor, clear screen/lines and control cursor visibility

#### Example

```bash
# Move cursor up 2 lines
sdk:cursor up 2
```

#### Options

* up Move cursor up N lines
* down Move cursor down N lines
* right Move cursor right N columns
* left Move cursor left N columns
* next Move cursor to beginning of next line
* prev Move cursor to beginning of previous line
* line Move cursor to column N of current line
* pos Move cursor to line N, column M
* clear Clear entire screen
* clear-line Clear current line
* clear-line-end Clear from cursor to end of line
* clear-line-start Clear from cursor to start of line
* clear-screen Clear screen and move cursor to home
* save Save cursor position
* restore Restore cursor position
* hide Hide cursor
* show Show cursor

#### Arguments

* **$1** (Command): - The cursor command to execute
* **$2** (Lines/Columns): - Number of lines/columns for movement commands (optional, defaults to 1)
* **$3** (Column): - Column number for 'pos' command (optional, defaults to 1)

#### Exit codes

* **0**: If successful
* **1**: If invalid command provided

#### Output on stdout

* ANSI escape sequences for cursor control

#### See also

* [echo](#echo)

