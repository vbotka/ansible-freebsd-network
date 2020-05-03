# freebsd_network

[![Build Status](https://travis-ci.org/vbotka/ansible-freebsd-network.svg?branch=master)](https://travis-ci.org/vbotka/ansible-freebsd-network)

[Ansible role.](https://galaxy.ansible.com/vbotka/freebsd_network/) FreeBSD. Configure network.

Please feel free to [share your feedback and report issues](https://github.com/vbotka/ansible-freebsd-network/issues). Contributions are welcome.


## Requirements

None.


## Role Variables

Review the defaults and examples in vars.


## Dependencies

None.


## Workflow

1) Change shell to /bin/sh

```
shell> ansible host -e 'ansible_shell_type=csh ansible_shell_executable=/bin/csh' -a 'sudo pw usermod user -s /bin/sh'
```

2) Install role

```
shell> ansible-galaxy install vbotka.freebsd_network
```

3) Fit variables

```
shell> editor vbotka.freebsd_network/vars/main.yml
```

4) Create playbook

```
shell> cat freebsd-network.yml
- hosts: host
  roles:
    - vbotka.freebsd_network
```

5) Configure the system

```
shell> ansible-playbook freebsd-network.yml
```


## References

- [FreeBSD handbook: 11.5. Setting Up Network Interface Cards](https://www.freebsd.org/doc/handbook/config-network-setup.html)
- [FreeBSD handbook: 11.6. Virtual Hosts](http://www.freebsd.org/doc/handbook/configtuning-virtual-hosts.html)
- [FreeBSD handbook: 31.2. Gateways and Routes](https://www.freebsd.org/doc/handbook/network-routing.html)
- [FreeBSD handbook: 31.3. Wireless Networking](http://www.freebsd.org/doc/handbook/network-wireless.html)
- [FreeBSD handbook: 31.6. Bridging](https://www.freebsd.org/doc/handbook/network-bridging.html)
- [FreeBSD handbook: 31.7. Link Aggregation and Failover](https://www.freebsd.org/doc/handbook/network-aggregation.html)
- [FreeBSD handbook: 31.9. IPv6](http://www.freebsd.org/doc/handbook/network-ipv6.html)
- [FreeBSD handbook: 31.10. Common Address Redundancy Protocol (CARP)](http://www.freebsd.org/doc/handbook/carp.html)
- [FreeBSD handbook: 31.11. VLANs](http://www.freebsd.org/doc/handbook/network-vlan.html)


## License

[![license](https://img.shields.io/badge/license-BSD-red.svg)](https://www.freebsd.org/doc/en/articles/bsdl-gpl/article.html)


## Author Information

[Vladimir Botka](https://botka.link)
