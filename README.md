# Raw Mbed project for libcose and suit

# Getting started

To be able to build with mbed compile, first modify tinycbor:

```sh
cp tinycbor/src/cbor.h tinycbor/
```

Then modify libcose:

```sh
sed -i'' -e 's|cbor.h|tinycbor/cbor.h|' libcose/include/cose/cbor.h
```

Now, you should be able to compile.