Mellanox SAI implementation
============================

This repository contains SAI implementation for Mellanox hardware.

SAI headers are based on latest head (as of Feb 22, 2018) of branch v1.2 (following release v1.2.3) SAI headers can be 
downloaded from https://github.com/opencomputeproject/SAI/

The implementation is written over Mellanox SwitchX interfaces API. The API and documentation for it, are available in
https://github.com/Mellanox/SwitchX-interfaces

Compilation is done with the flag USE_SAI_INTERFACE=1
For example : make all_native USE_KERNEL=0 USE_SAI_INTERFACE=1
The output result is SAI library, called libsai.

User applications can then link with this library, in order to use the SAI implementation.
