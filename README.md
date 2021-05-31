
# A Heka file reader

[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/ZeitgeberH/HekaReader/issues)&nbsp;



### Usage
```python
## import main reader 
import HEKA_Reader_MAIN as HEKA
## import wrapper
from HekaHelpers import HekaBundleInfo

## read Heka .dat file into a object
bundleTester = HekaBundleInfo(makePath(DataPath, testFile))

## Get sample rate
traceIndex = [0,0,0,0]
bundleTester.getSeriesSamplingRate(traceIndex)
```

