For the ease of distribution, such as bundle in the factory/recovery tool,
it's nice to have a static-linked version.

The following command install static version of libusb and libpthread On Gentoo Linux.
```
sudo USE=static-libs emerge libpthread-stubs
```

Build
```
LDFLAGS="-static -pthread" ./configure
make -j8
```
