LZVN
====

You can download the source code of LZVN and pre-compiled copies of libFastCompression.a and libFastCompression-Kernel.a with:

``` sh
curl -o LZVN.zip https://codeload.github.com/Piker-Alpha/LZVN/zip/master
```


Unzip
-----

You can unzip the downloaded archive with:

```
unzip -qu LZVN.zip [-d target directory]
```


Make instructions
-----------------

```
make
``` 

Note: You don't need to run: ```make clean``` first because that is done automatically.


Installation
------------

You can install the executable with:

```
make install
```

Note: The executable will be copied to: /usr/local/bin


Usage
-----

```
./lzvn <uncompressed filename> <compressed filename>
./lzvn -d <compressed filename> <uncompressed filename>
./lzvn -d <path/prelinkedkernel> kernel
./lzvn -d <path/prelinkedkernel> dictionary
./lzvn -d <path/prelinkedkernel> kexts
```

The third option will extract the kernel from the given prelinkedkernel.
The fourth option will extract the dictionary containing the Info.plist of all kexts.
The last option will extract all kexts in its current format, saved in subdirectory with the name kexts.


Bugs
----

All possible bugs (so called 'issues') should be filed at:

https://github.com/Piker-Alpha/LZVN/issues

Please do **not** use my blog for this. Thank you!

