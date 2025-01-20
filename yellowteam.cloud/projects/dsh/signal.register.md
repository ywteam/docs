# signal.register.sh

Register signal handlers for specified signals

## Overview

Registers signal handlers for the specified signals. If a signal is
already trapped, displays a warning message.

## Index

* [dsh:signal:register](#dshsignalregister)

## signal

### dsh:signal:register

Registers signal handlers for the specified signals. If a signal is
already trapped, displays a warning message.

#### Example

```bash
dsh:signal:register SIGTERM SIGINT
# Registers handlers for SIGTERM and SIGINT signals
```

#### Arguments

* **...** (List): of signals to register handlers for (e.g., SIGTERM, SIGINT)

#### Exit codes

* **0**: Always successful
* **1**: If failed to register signal handler

#### See also

* [dsh:log:warn Logs warning messages if signal already trapped](#dshlogwarn-logs-warning-messages-if-signal-already-trapped)
* [dsh:on:signal Signal handler function that gets called when signal received](#dshonsignal-signal-handler-function-that-gets-called-when-signal-received)
* [dsh:style Function to style text output](#dshstyle-function-to-style-text-output)

