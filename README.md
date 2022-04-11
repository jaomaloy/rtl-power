# rtl-power
Gather radio frequency data with this balena block and an RTL_SDR. [Rtl_power](http://kmkeen.com/rtl-power/) is a unix-hacker's approach to the waterfall spectrum that radio amateurs are familiar with, please check it's webpage to see usecases. This block is simply an abstraction for it and sets sane defaults for IoT.

##### Supported environment variables
- `LOWER_BAND` - The lowest frequency band to sample.
- `UPPER_BAND` - The highest frequency band to sample.
- `BIN_SIZE` - The size of each frequency sampling bin.
- `INTERVAL` - Change this value to change the sampling interval. Include short hand time modifiers such as *s* for seconds, *m* for minutes, *h* for hours. The default interval is 10 seconds (10s).
- `TUNER_GAIN` - Change this value to change the gain. Default is automatic configuration based on the connected dongle.

To edit these values in the dashboard, simply press `Variables` on the left column.
