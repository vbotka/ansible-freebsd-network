========================================
vbotka.freebsd_network 2.7 Release Notes
========================================

.. contents:: Topics


2.7.5
=====

Release Summary
---------------
Notify 'restart netif && restart routing' on changes.


2.7.4
=====

Release Summary
---------------
Remove .ansible dir. Add .gitignore


2.7.3
=====

Release Summary
---------------
Remove var fn_ethname_cmd from ethname task name.


2.7.2
=====

Release Summary
---------------
Add ethname debug.


2.7.1
=====

Release Summary
---------------
Bugfix update. Fix ethname.


2.7.0
=====

Release Summary
---------------
Major release. Requires collections community.general and vbotka.freebsd

Major Changes
-------------
* Meta: Ansible 2.18; FreeBSD 13.4, 13.5, 14.2
* Enable configuration in rc.conf.d
  Added vars: fn_rcconfd (default=false), fn_rcconfd_dir (default=/etc/rc.conf.d)
* Added ethname MAC-based network name pinning
  Install sysutils/ethname
  Added vars: fn_ethname (default=false), fn_ethname_enable (default=false) ...
  Added sample in vars/mainlyml.sample
* Module ansible.builtin.service replaced by vbotka.freebsd.service
* Module ansible.builtin.lineinfile replaced by community.general.sysrc

Minor Changes
-------------

Bugfixes
--------

Breaking Changes / Porting Guide
--------------------------------
