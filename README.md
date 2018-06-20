# Lineage buildscripts
========================

Starting from zero:
---------
    mkdir -p ~/android/lineage
    cd ~/android/lineage
    repo init -u git://github.com/LineageOS/android.git -b cm-14.1
    mkdir -p .repo/local_manifests
    curl https://raw.githubusercontent.com/lineage-n-asus-Z00XS/local_manifests/cm-14.1/local_manifest.xml > .repo/local_manifests/my_manifest.xml
    repo sync

If you've already synced Lineage-Sources:
----------
    mkdir -p .repo/local_manifests
    curl https://raw.githubusercontent.com/lineage-n-asus-Z00XS/local_manifests/cm-14.1/local_manifest.xml > .repo/local_manifests/my_manifest.xml
    repo sync

Building
----------
    cd /path/to/lineage
    curl https://raw.githubusercontent.com/lineage-o-x2/local_manifests/cm-14.1/clean_Z00XS_build.sh > clean_Z00XS_build.sh
    curl https://raw.githubusercontent.com/lineage-o-x2/local_manifests/cm-14.1/dirty_Z00XS_build.sh > dirty_Z00XS_build.sh
    . clean_Z00XS_build.sh // for clean builds
    . dirty_Z00XS_build.sh // for dirty builds

I made these modified scripts for convenience plus logs terminal output to files for easy scrolling later in your favorite text editor.
