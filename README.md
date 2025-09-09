# ogn-rf-soapysdr
SoapySDR based RF front for the OGN receiver

## re-import of project without binary blobs
Upstream had build artifacts in the source repository, so we used bfg to remove
those files and re-import the project without them.

This retains the commit history but rewrites the commit hashes.
Something usually you tend to avoid, but as upstream did not seem to have any
changes for a long time, this was the best option.

Used command:
```sh
bfg -D '*.tgz' --no-blob-protection ogn-rf-soapysdr.git
```