Commands that successfully built something at some point
========================================================

gdb-multiarch with python support
---------------------------------

```
cd <GDB_SOURCE>
./configure --enable-target=all --with-python
make
```

Debuggable linux kernel, using buildroot
----------------------------------------

```
cd <BUILDROOT_SOURC>

# Configure linux. Make sure to enable "Compile kernel with debugging symbols"
make linux-menuconfig

# Configure toolchain. Make sure to disable optimizations. Chose target arch,
# etc.
make menuconfig
```
