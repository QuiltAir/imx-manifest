Quilt Repo Manifest README
==========================

This repo is used to download manifests for Quilt BSP releases.

Install the `repo` utility:
---------------------------

To use this manifest repo, the `repo` tool must be installed first.

```
$: mkdir ~/bin
$: curl http://commondatastorage.googleapis.com/git-repo-downloads/repo  > ~/bin/repo
$: chmod a+x ~/bin/repo
$: PATH=${PATH}:~/bin
```

Install essential host packages
------------------------------
Your Build Host must install required packages for the Yocto build.
Reference to the section "Build Host Packages" in the document "Yocto Project Quick build".
- https://docs.yoctoproject.org/5.0.3/brief-yoctoprojectqs/index.html#build-host-packages

Download the Yocto Project BSP
------------------------------

```
$: repo init -u https://github.com/QuiltAir/imx-manifest -b quilt -m quilt-6.6.23-2.0.0.xml
$: repo sync
```
