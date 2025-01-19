# cleanup.sh

System package manager cleanup utility

## Overview

This function performs cleanup operations across various package managers
in the system. It attempts to clean package caches and remove unnecessary files
for each detected package manager.

## Index

* [sdk:cleanup](#sdkcleanup)

## cleanup

### sdk:cleanup

This function performs cleanup operations across various package managers
in the system. It attempts to clean package caches and remove unnecessary files
for each detected package manager.

#### Example

```bash
sdk:cleanup
```

_Function has no arguments._

#### Exit codes

* **0**: Always returns success

#### Output on stdout

* Information about cleanup operations being performed

#### Output on stderr

* Possible errors from package managers or cleanup commands

#### See also

* [sdk:log:stdin](#sdklogstdin)

