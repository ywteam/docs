# signal.register.sh

Register signal handlers for specified signals

## Overview

Registers signal handlers for the specified signals. If a signal is
already trapped, displays a warning message.

## Index

* [sdk:signal:register](#sdksignalregister)

## signal

### sdk:signal:register

Registers signal handlers for the specified signals. If a signal is
already trapped, displays a warning message.

#### Example

```bash
sdk:signal:register SIGTERM SIGINT
# Registers handlers for SIGTERM and SIGINT signals
```

#### Arguments

* **...** (List): of signals to register handlers for (e.g., SIGTERM, SIGINT)

#### Exit codes

* **0**: Always successful
* **1**: If failed to register signal handler

#### See also

* [sdk:log:warn Logs warning messages if signal already trapped](#sdklogwarn-logs-warning-messages-if-signal-already-trapped)
* [sdk:on:signal Signal handler function that gets called when signal received](#sdkonsignal-signal-handler-function-that-gets-called-when-signal-received)
* [sdk:style Function to style text output](#sdkstyle-function-to-style-text-output)

