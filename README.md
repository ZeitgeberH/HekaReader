
# A Heka file reader

[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/ZeitgeberH/HekaReader/issues)&nbsp;



### Usage
```python
## import HekaHelpers which is a wrapper of main file: HEKA_Reader_MAIN
from HekaHelpers import HekaBundleInfo

## read Heka .dat file into a object
bundleTester = HekaBundleInfo(makePath(DataPath, testFile))

## Get sample rate
traceIndex = [0,0,0,0] ## [Group, Series, Sweep, Trace]
bundleTester.getSeriesSamplingRate(traceIndex)

## Get stimuli information
traceIndex = [0,0,0,0]
time, stim, stimInfo = bundleTester.getStim(traceIndex)

## Get data from a single sweep and single channel
traceIndex = [0,0,0,0]
data = bundleTester.getSingleTraceData(traceIndex)
```

