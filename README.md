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
