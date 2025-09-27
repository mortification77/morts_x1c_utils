# Mort's X1(C) Utils
## Various Utilities for the Bambu X1(C) Series 3D Printer

### This repository contains custom 3D Printer utilities and files for the Bambu Labs X1(C) Series Printer.

> ### WARNING: Use at *your own risk!*

---

## Bed Leveling (Directory: *bed_level/*)

> ### The default hotbed_tramming_20221102.gcode file provided by Bambu is a "destructive" bed level procedure meaning that it cannot be repeated for further fine tuning or validation as the bed screws must be adjusted each time before executing.
>
> ### The modifications contained within this repository will allow for repeat leveling without touching the bed screws before each level.
>
> ### **NOTE: It is still HIGHLY RECOMMENDED to even them out before running this gcode.**


### Files

* bed_level/hotbed_tramming_mort_30s.gcode

	- Updated "G1 ZX.X" moves to move up only 0.1 mm (instead of 0.4 mm) from the bed for each adjustment position.

		+ Allows use of the "paper technique" instead of feeler gauges or looking at the nozzle as the rear adjustment is exceptionally difficult to perform using either of these methods.

		+ Allows re-running of the tramming routine without having to adjust the bed screws first.
		
	- Updated wait time from 15 seconds to 30 seconds on subsequent pauses to give additional time for testing and adjusting.

		+ The original waited for 30 seconds for the initial adjustment but dropped down to 15 seconds for subsequent pauses.

