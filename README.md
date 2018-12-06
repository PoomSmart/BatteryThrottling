# BatteryThrottling
[WIP] Battery throttling activation on some unsupported iOS versions.

Inside `/System/Library/Watchdog/ThermalMonitor.bundle/<model>.bundle/Info.plist` where `<model>` is your device internal model name (`N69uAP`, for example), there is a dictionary called `generalProductConfig`. There is one interesting key that you can add in order to disable battery throttling: `skipMitigationController` as a boolean.

Have not tried personally. Might do at some point.
