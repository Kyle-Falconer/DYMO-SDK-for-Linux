
About
-----
This is a fork of the official [DYMO SDK for Linux, version 1.4.0.5](http://www.dymo.com/en-US/dymo-label-sdk-and-cups-drivers-for-linux-dymo-label-sdk-cups-linux-p--1), which was last updated in 2012 for CUPS version 1.4.6. This official version no longer compiles with CUPS v2 or higher. Attempts to ask DYMO Customer Support about updates to this driver have failed, as they longer support the Linux operating system.

The fix for this comes as a patch found on a [forum post](https://ubuntuforums.org/showthread.php?t=2376862&styleid=118) regarding the same issue.

Installation:
-------------
```bash
sudo apt-get install libcups2-dev libcupsimage2-dev gcc g++ automake
automake
autoconf
./configure
make
sudo make install
```
						
Command examples:
-----------------

- print very long text on a tape:
```
lpr -o landscape -o PageSize=24_mm__1___Label__Auto_ docs/test.txt
```

- set printing options specific to the LabelWriter driver
```
lpr -o PageSize=30252_Address -o PrintQuality=Graphics -o PrintDensity=Light docs/test.txt
```

- set printing options specific to the LabelManager driver
```
lpr -o PageSize=Address_Label -o CutOptions=ChainMarks -o LabelAlignment=Right -o TapeColor=1
```
