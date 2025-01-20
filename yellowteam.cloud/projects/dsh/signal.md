# signal.sh

Lists all currently set traps

## Overview

Lists all currently set traps by using trap -p command and
extracting signal names using awk. Each signal name is written
to file descriptor 7.


