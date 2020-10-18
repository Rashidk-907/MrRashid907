
# daemaged.compression.native

An amalgamation of:
* zlib (zlib-ng)
* bzip
* liblzma
* lzo2
* lz4 
* zstd
native compression libs into one .NET Wrapper for .NET Core

This repo holds refs to the various compression libraries unser the src folder, and the azure devops pipeline tha
spins up docker images to build these libraries for the following OS / .NET RIDs:
* ubuntu.14.04
* ubuntu.16.04
* ubuntu.18.04
* debian.9
* rhel.7

and package the entire output under the Daemaged.Compression.Native nuget package.

Users should **not** consume this library directly, but should rather use the Daemaged.Compression library, that has a
dependency on nuget produced by these repo.
