---
description: Loadable Kernel Modules
---

# LKMs

### Functionality

* Expand linux kernel
* Loaded dynamically

### Basic Function

* OLD
  * int init\_module(void) {}
    * non 0 return value --> the module can't be loaded
  * void cleanup\_module(void) {}
* NEW
  * static int \_\_init init\_func(void) {}
  * static void _\_\_exit_ exit\_func(void) {}
  * module\_init(init\_func);
  * module\_exit(exit\_func);
* MODULE\_LICENSE("GPL");

### Makefile

* $(CURDIR) --> set abs pathname to current working directory
  * sudo make may go wrong if PWD is not set to CURDIR
* Reference
  * [gnu make manual](https://www.gnu.org/software/make/manual/make.html)
