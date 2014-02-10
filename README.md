AOSP 4.4.2 KitKat for Galaxy S4
=============================

Current status: Release Candidates



Download:
----------
* mkdir ~/AOSP
* cd ~/AOSP
* repo init -u git://github.com/AOSP-S4-KK/platform_manifest -b kk-4.4
* repo sync



Building:
----------
* . build/envsetup.sh
* lunch
* make otapackage

(after doing 'make clean' you need to lunch again before rebuilding)



Fixing 'lz4c' not found:
------------------------

Due to new lossless kernel compression (LZ4), the lz4c binary is needed until properly implemented in the rom tree. This can be installed by following the steps below:

- wget http://lz4.googlecode.com/files/lz4-r112.tar.gz
- tar -xf lz4-r112.tar.gz
- cd lz4-r112
- make
- sudo make install
