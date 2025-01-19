# io.read.region.sh

Read region from file

## Overview

Read region from file

## Index

* [sdk:io:region:read](#sdkioregionread)

### sdk:io:region:read

Read region from file

#### Example

```bash
# all output
sdk:io:region:read "file" "region" >&7     
# just region content
sdk:io:region:read "file" "region" >&7 | head -n -1
# just the lines numbers
sdk:io:region:read "file" "region" >&7 | tail -n 1
# read lines as array
readarray -t lines < <(sdk:io:region:read "file" "region" >&7 | head -n -1)
read -a lines < <(sdk:io:region:read "${file}" "${region}" >&7 | head -n -1)
```

#### Exit codes

* **0**: If successful, 1 otherwise

#### Output on stdout

* Region content. The last line of the output is the end line

