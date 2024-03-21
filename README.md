# python `aer` library

A library for reading ".aedat" files for logging outputs from
[DVS event-based cameras](https://inivation.com/dvs/).

Fork - When opening old datasets like [DVS128 Gestures](https://paperswithcode.com/dataset/dvs128-gesture-dataset) most libraries seem to be too modern. This repo was the most compact that I could find/edit to my needs.

# How to install

```
git clone https://github.com/cocoalex00/python-aerpy.git
cd python-aerpy
python setup.py install
```

# How to use

```
import aer

# read all at once
events = aer.AEData("mylogfile.aedat")

# read only the first 1000 events in the file
events = aer.AEData("mylogfile.aedat", n=1000)

```

# License

MIT
