
How to build:
-------------

Initialize repo:

    repo init -u git://codeaurora.org/platform/manifest.git -b release --depth 1 -m LA.BF.1.1.3-01610-8x74.0.xml --repo-url=git://codeaurora.org/tools/repo.git --repo-branch=caf-stable
    curl --create-dirs -L -o .repo/local_manifests/local_manifest.xml -O -L https://raw.githubusercontent.com/nx503a/android_local_manifest/mm/local_manifest.xml
    repo sync -j16

Compile:

    . build/envsetup.sh
    lunch aosp_device-userdebug
    make otapackage

This is a memo for compilation of omnirom.
