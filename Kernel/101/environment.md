---
description: Set up an environment for kernel dev
---

# Environment

Reference: [mgalas](https://mgalgs.io/2021/03/23/how-to-build-a-custom-linux-kernel-for-qemu-using-docker.html)

* busybox
  * alternative for linux core util
* initramfs
  * defines the booting process
  * often compressed as cpio
  * inspection
    * lsinitrd
    * lsinitramfs
    * extract initramfs with cpio ([detail](https://wiki.debian.org/initramfs))
