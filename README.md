# KAT files for SNOVA Round 2

This repository contains the offical KAT files for SNOVA as submitted to Round 2 of the NIST competition.

Note:
The .rsp files of SNOVA_75_33_16_2_ESK and SNOVA_75_33_16_2_SHAKE_ESK are compressed as the original KAT files are over the file size limit of github.
Use `gunzip` to obtain the actual .rsp files.

## SHAKE256 KAT digests

The file KAT-SHAKE256 in this folder contains the 64 byte SHAKE256 digests of the uncompressed KAT response (.rsp) files.
The reqest (.req) file is identical for all parameter sets.

To generate a digest use e.g.
```
openssl dgst -shake256 -xoflen=64 SNOVA_37_17_16_2_ESK/PQCsignKAT_SNOVA_37_17_2_ESK.rsp
```

This will output
```
SHAKE-256(SNOVA_37_17_16_2_ESK/PQCsignKAT_SNOVA_37_17_2_ESK.rsp)= cd5f1711dbc6a780effc5e0a2b97af92880c643be1640188eded8cd52c3f3efbdbdf417f43f006ddf1d5b0dc690cd21ce58e18daac30547a1494e78f8f25287c
```
