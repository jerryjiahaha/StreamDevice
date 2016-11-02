EPICS StreamDevice
==================

[Official website](http://epics.web.psi.ch/software/streamdevice/doc/index.html)

[Official repo](https://github.com/paulscherrerinstitute/StreamDevice)

I just add some codes for my lab's project and try to learn this project.

I made the directory structure modular ( like epics modules such as asyn, calc, etc ).

Tested on linux-x86\_64 with base 3.14.12.5

Setup
-----
1. Modify env. See `configure/RELEASE`, set BASE and modules ASYN, CALC. You can override `SUPPORT`, `ASYN`, `CALC`, `EPICS_BASE` in `SUPPORT.$(EPICS_HOST_ARCH)` and `EPICS_BASE.$(EPICS_HOST_ARCH)` out of the project.

2. Set `INSTALL_LOCATION` in `configure/CONFIG_SITE`. This is optional, I use env `BASE_SUPPORT_PATH` to set epics modules' path. The project will be installed into `${BASE_SUPPORT_PATH}/stream` if this env is defined.

3. Just calling `make`.
