# bundle.validate.sh

Validates shell script bundles for SDK compliance

## Overview

Validates a shell script bundle to ensure it follows SDK standards:
1. Checks for explicit exit codes in the script
2. Sources the script and verifies it loads without errors
3. Ensures all declared functions use the sdk: namespace prefix


