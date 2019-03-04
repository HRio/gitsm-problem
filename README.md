small repo to show how gitsm in Yocto Thud fails with recursive submodules


Example gitsm-problem.bb
```
SUMMARY = "Reproduce gitsm problem"
SECTION = "base"
LICENSE = "Other"
PR	= "r1"

LIC_FILES_CHKSUM += "file://external/google-fonts/apache/robotocondensed/LICENSE.txt;md5=3b83ef96387f14655fc854ddc3c6bd57"

SRCREV = "eae8f650123c6419197dec2418c1425a8f7fa016"

SRC_URI = "gitsm://git@github.com/HRio/gitsm-problem.git;protocol=ssh;branch=master"

S = "${WORKDIR}/git"
```
