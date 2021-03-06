puppet-libvirt
======

Puppet module for managing libvirt configurations.

#### Table of Contents
1. [Overview - What is the libvirt module?](#overview)
2. [Usage](#usage)

Overview
--------

This module is used to install and configure libvirt.

Usage
-----

Parameters:
* **virt_type**: the virtualization type, currently only 'kvm' is supported
* **vnc_listen**: set this to '0.0.0.0' to enable public VNC access
* **vnc_password**: set the VNC password

**Configuring libvirt**

```libvirt
class {'libvirt':
    virt_type    => 'kvm',
    vnc_listen   => "0.0.0.0",
    vnc_password => "mysafepass",
}
```

Contributors
------------

* https://github.com/desalvo/puppet-libvirt/graphs/contributors

Release Notes
-------------

**0.1.0**

* Initial version
