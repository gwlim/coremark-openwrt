CoreMark for OpenWrt
====================

Original Source: https://github.com/eembc/coremark
--------------------------------------------------

How to use
----------

* copy the coremark folder to openwrt/package/utils

![alt text](https://raw.githubusercontent.com/gwlim/coremark-openwrt/master/coremark.png)

make menuconfig

Select

* Utilities > coremark

Save and make

    make package/coremark/compile

Sample Test Run for AR9344 (mips74k) WDR4300v1
----------------------------------------------

```
root@openwrt:/tmp# ./coremark 
2K performance run parameters for coremark.
CoreMark Size    : 666
Total ticks      : 16982
Total time (secs): 16.982000
Iterations/Sec   : 1766.576375
Iterations       : 30000
Compiler version : GCC6.4.0
Compiler flags   : -O2   -lrt
Memory location  : Please put data memory location here
			(e.g. code in flash, data on heap etc)
seedcrc          : 0xe9f5
[0]crclist       : 0xe714
[0]crcmatrix     : 0x1fd7
[0]crcstate      : 0x8e3a
[0]crcfinal      : 0x5275
Correct operation validated. See readme.txt for run and reporting rules.
CoreMark 1.0 : 1766.576375 / GCC6.4.0 -O2   -lrt / Heap
```

