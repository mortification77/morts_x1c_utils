# Mort's X1(C) Utils
## Various Utilities for the Bambu X1(C) Series 3D Printer

### This repository contains custom 3D Printer utilities and files for the Bambu Labs X1(C) Series Printer.

---

#### Bed Leveling (Directory: *bed_level/*)

> The default hotbed_tramming_20221102.gcode file provided by Bambu is a "destructive" bed level procedure meaning that it cannot be repeated for further fine tuning or validation as the bed screws must be adjusted each time before executing.

> The modifications contained within this repository will allow for repeat leveling without touching the bed screws before each level.

> **NOTE: It is still HIGHLY RECOMMENDED to even them out before running this gcode.**


## Files

* hotbed_tramming_mort_30s.gcode
	- Updated to move up only 0.1mm (instead of 0.4mm) from the bed (allows for "paper" leveling).
	- Updated wait time from 15s to 30s on subsequent pauses to give additional time for testing and adjusting.
		+ The original waited for 30s for the initial adjustment but dropped down to 15s for subsequent pauses.

