# io.write.region.sh

Write content to region in file

## Overview

Write content to region in file

## Index

* [dsh:io:region:write](#dshioregionwrite)

### dsh:io:region:write

Write content to region in file

#### Example

```bash
dsh:io:region:write "file" "region" "content"
dsh:io:region:write "file" "region" "content" >&7
dsh:io:region:write "file" "region" "content" >&7 | dsh:log:stdin "debug"
```

#### Exit codes

* **0**: If successful, 1 otherwise
* **1**: If file does not exist
* **2**: If region is empty
* **3**: If start or end line is empty
* **4**: If start or end line is not a number
* **5**: If failed to write region to file

#### See also

* [io.read.region](#ioreadregion)

