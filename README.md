# vmw-logger-rs
A VMware logger rust crate that leverages an undocumented built-in backdoor for guest-host interaction with no_std support.

### How to enable
To enable this functionality, add the following lines to the *.VMX file:
```
replay.enableBackdoorPutChar = "TRUE"
log.guestThrottleBytesPerSec = "100000000"
log.throttleBytesPerSec = "100000000"
log.append = "FALSE"
log.keep = "FALSE"
```

### Credits
- jessie (intege_rs)
- YushiOMOTE
