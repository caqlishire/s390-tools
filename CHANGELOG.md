Release history for s390-tools (MIT version)
--------------------------------------------

 * __v2.3.1 (XXX-XX-XX)__

  For Linux kernel version: 4.16

  Changes of existing tools:
  - dbginfo: Gather nvme related data

  Bug Fixes:

* __v2.3.0 (2018-01-30)__

  For Linux kernel version: 4.15

  Changes of existing tools:
  - lscpumf: Add support for IBM z14 hardware counters
  - libdasd: Introduce libdasd and use for dasd tools
  - zipl: Always build and link without PIE

  Bug Fixes:
  - zgetdump: Fix handling of DASD multi-volume dump for partitions above 4 GB
  - zdev: Fix zdev dracut module aborting on unknown root device

* __v2.2.0 (2017-12-07)__

  For Linux kernel version: 4.14

  Removed tools:
  - lsmem/chmem: Moved to util-linux >= 2.30

  Changes of existing tools:
  - lszcrypt: Add CEX6S support
  - cpuplugd/mon_tools: Improve systemctl start error handling
  - systemd: Install also the unit configuration files

  Bug Fixes:
  - build process: Fix parallel build for libutil
  - cpi: Add missing Install section to service unit
  - lsluns: Do not scan (all) if filters match nothing
  - lsluns: Enhance usage statement and man page
  - zdev: Use correct path to vmcp binary
  - ziomon: Re-add missing line in ziomon_fcpconf
  - ziomon: Fix non-zero return code in ziomon_util
  - zipl: Remove invalid dasdview command line option

* __v2.1.0 (2017-09-25)__

  For Linux kernel version: 4.13

  Added new tools:
  - netboot: Scripts for building a PXE-style netboot image for KVM
  - 90-cpi.rules/cpictl: New udev rule to update CPI when KVM is used

  Changes of existing tools:
  - lsqeth/zdev: Add VNIC Characteristics support

  Bug Fixes:
  - chzcrypt: Corrected handling of insufficient permissions
  - cpacfstats: Add size setting to perf event
  - fdasd: Skip partition check with the force option
  - ttyrun: Fix deprecated BindTo usage in ttyrun-getty@.service.in
  - lszcrypt: Fix core dump caused by stack overwrite
  - lszcrypt: Fix random domain printout when no config available
  - zdev: Fix segfault with unknown qeth attribute
  - zdev: Fix IPv6 NDP proxy description
  - zdev: Fix zdev dracut module temp file location
  - zkey: Correctly detect abbreviated commands
  - zkey: Validate XTS key: ignore domain and card
  - zkey: Use octal values instead of S_IRWX* constants
  - zkey: Properly set umask to prohibit permissions to group and others
  - zkey: Add -ldl to LDLIBS (not LDFLAGS)
  - znetconf: Re-add missing line in lsznet.raw
  - Fix several gcc 7 warnings

* __v2.0.0 (2017-08-21)__

  - Publish package under the MIT license with the same contents as
    the already available s390-tools-1.39.0

Previous releases of s390-tools can be found on the IBM Developer Works
web pages:

  - https://www.ibm.com/developerworks/linux/linux390/s390-tools.html
