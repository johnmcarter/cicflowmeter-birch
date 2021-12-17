# cicflowmeter-birch

This repo contains source code for a network sensor to track packet flows on Linux distributions. The original source code can be found at https://gitlab.com/hieulw/cicflowmeter/-/tree/master/src/cicflowmeter. Since there are persistent bugs in the source code, this repo was created as a workaround so that the PyPi package can be used and work correctly.

## Installation
Install cicflowmeter from PyPi and clone this repo:
```
pip3 install cicflowmeter
git clone https://github.com/johnmcarter/cicflowmeter-birch.git
```

Then overwrite the source files from the pip install:
```
cp -r cicflowmeter-birch/*  /usr/local/lib/python3.9/dist-packages/cicflowmeter/
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


Last modified: 15 December 2021
Last tested on: October 2021 release of Raspberry Pi OS