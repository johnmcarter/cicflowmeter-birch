# cicflowmeter-birch

This repo contains a network sensor to track packet flows on Linux distributions. The original source code can be found at https://gitlab.com/hieulw/cicflowmeter/-/tree/master/src/cicflowmeter. This repo was forked because there are persistent bugs in the original source code that aren't fixed.

## Installation
```
git clone https://github.com/johnmcarter/cicflowmeter-birch.git
cd cicflowmeter-birch
python3 setup.py install
```

## Usage
```
usage: cicflowmeter [-h] (-i INPUT_INTERFACE | -f INPUT_FILE) [-c] [-u URL_MODEL] output

positional arguments:
  output                output file name (in flow mode) or directory (in sequence mode)

optional arguments:
  -h, --help            show this help message and exit
  -i INPUT_INTERFACE    capture online data from INPUT_INTERFACE
  -f INPUT_FILE         capture offline data from INPUT_FILE
  -c, --csv, --flow     output flows as csv
```

## Reference 
https://www.unb.ca/cic/research/applications.html#CICFlowMeter