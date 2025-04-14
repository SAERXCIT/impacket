Merged PRs
==========

* [#1137](https://github.com/SecureAuthCorp/impacket/pull/1137): Add SystemDPAPIdump.py example
* [#1161](https://github.com/SecureAuthCorp/impacket/pull/1161): Implement Kerberos authentication for HTTP
* [#1202](https://github.com/SecureAuthCorp/impacket/pull/1202): Added `-self` and `-altservice` to getST for S4U2self abuse and service substitution
* [#1224](https://github.com/SecureAuthCorp/impacket/pull/1224): Added renameMachine.py
* [#1253](https://github.com/SecureAuthCorp/impacket/pull/1253): Make default ntlmrelayx dump SAM and LSA
* [#1262](https://github.com/SecureAuthCorp/impacket/pull/1262): [secretsdump] Added parsing of services passwords (SCM)
* [#1288](https://github.com/SecureAuthCorp/impacket/pull/1288): [ntlmrelayx] LDAP attack: bypass computer creation restrictions with CVE-2021-34470
* [#1395](https://github.com/SecureAuthCorp/impacket/pull/1395): Correctly include authtime and etype in ticket conveter
* [#1402](https://github.com/SecureAuthCorp/impacket/pull/1402): Add Shadow Credentials Commands to Ntlmrelayx's Interactive LDAP Shell
* [#1425](https://github.com/SecureAuthCorp/impacket/pull/1425): Add SCCM NTLM Relay Attack
* [#1428](https://github.com/SecureAuthCorp/impacket/pull/1428): [ntlmrelayx/adcs] Encode and handle non-alphanumeric chars in CertificateName
* [#1431](https://github.com/SecureAuthCorp/impacket/pull/1431): Update ccache.py to enhance the ability of dealing with cross realm ticket
* [#1442](https://github.com/SecureAuthCorp/impacket/pull/1442): Adds relay to ICPR over RPC
* [#1458](https://github.com/SecureAuthCorp/impacket/pull/1458): SID Bruteforce through ntlmrelay over SMB
* [#1462](https://github.com/SecureAuthCorp/impacket/pull/1462): Filter socks connections by Admin only
* [#1470](https://github.com/SecureAuthCorp/impacket/pull/1470): [secretsdump] Fix -use-vss for use in all languages
* [#1495](https://github.com/SecureAuthCorp/impacket/pull/1495): Fixing Kerberos Name Type in AS requests
* [#1477](https://github.com/SecureAuthCorp/impacket/pull/1477): Fix HKEY_CURRENT_USER and add HKEY_USERS
* [#1593](https://github.com/SecureAuthCorp/impacket/pull/1593): Feature/relay sccm adminservice
* [#1628](https://github.com/SecureAuthCorp/impacket/pull/1628): Patches secretsdump unable to compute Kerberos salt to retrieve AESkeys via Kerberos authentication
* [#1809](https://github.com/SecureAuthCorp/impacket/pull/1809): Add clear_keycredentiallinks to ldap_shell
* [#1813](https://github.com/SecureAuthCorp/impacket/pull/1813): bugfix in SEALKEY()
* [#1840](https://github.com/SecureAuthCorp/impacket/pull/1840): Add parsing for 'Export' hives and boot key computation from class names
* [#1847](https://github.com/SecureAuthCorp/impacket/pull/1847): Added user-status functionality to the SAMHashes Class of the secrestdump.py
* [#1875](https://github.com/SecureAuthCorp/impacket/pull/1875): add SAN with UPN by default when doing shadow credentials
* [#1893](https://github.com/SecureAuthCorp/impacket/pull/1893): Add support for binary entropy in dpapi.py unprotect
* [#1894](https://github.com/SecureAuthCorp/impacket/pull/1894): Fix: Add Ability to Read Files with Open Handles over SMB
* [#1895](https://github.com/SecureAuthCorp/impacket/pull/1895): [ psexecsvc.py ] New remote code execution tool
* [#1919](https://github.com/SecureAuthCorp/impacket/pull/1919): Support channel binding and ldap signing for ntlm and kerberos auth

Impacket
========

[![Latest Version](https://img.shields.io/pypi/v/impacket.svg)](https://pypi.python.org/pypi/impacket/)
[![Build and test Impacket](https://github.com/fortra/impacket/actions/workflows/build_and_test.yml/badge.svg)](https://github.com/fortra/impacket/actions/workflows/build_and_test.yml)

Copyright Fortra, LLC and its affiliated companies. All rights reserved.

Impacket was originally created by [SecureAuth](https://www.secureauth.com/labs/open-source-tools/impacket), and now maintained by Fortra's Core Security.

Impacket is a collection of Python classes for working with network
protocols. Impacket is focused on providing low-level
programmatic access to the packets and for some protocols (e.g.
SMB1-3 and MSRPC) the protocol implementation itself.
Packets can be constructed from scratch, as well as parsed from 
raw data, and the object-oriented API makes it simple to work with 
deep hierarchies of protocols. The library provides a set of tools
as examples of what can be done within the context of this library.

What protocols are featured?
----------------------------

 * Ethernet, Linux "Cooked" capture.
 * IP, TCP, UDP, ICMP, IGMP, ARP.
 * IPv4 and IPv6 Support.
 * NMB and SMB1, SMB2 and SMB3 (high-level implementations).
 * MSRPC version 5, over different transports: TCP, SMB/TCP, SMB/NetBIOS and HTTP.
 * Plain, NTLM and Kerberos authentications, using password/hashes/tickets/keys.
 * Portions/full implementation of the following MSRPC interfaces: EPM, DTYPES, LSAD, LSAT, NRPC, RRP, SAMR, SRVS, WKST, SCMR, BKRP, DHCPM, EVEN6, MGMT, SASEC, TSCH, DCOM, WMI, OXABREF, NSPI, OXNSPI.
 * Portions of TDS (MSSQL) and LDAP protocol implementations.
 
Maintainer
==========

[Core Security](https://www.coresecurity.com/)


Table of Contents
=================

* [Getting Impacket](#getting-impacket)
* [Setup](#setup)
* [Testing](#testing)
* [Licensing](#licensing)
* [Disclaimer](#disclaimer)
* [Contact Us](#contact-us)

Getting Impacket
================

### Latest version

* Impacket v0.12.0

  [![Python versions](https://img.shields.io/pypi/pyversions/impacket.svg)](https://pypi.python.org/pypi/impacket/)

[Current and past releases](https://github.com/fortra/impacket/releases)

### Development version

* Impacket v0.13.0-dev (**[master branch](https://github.com/fortra/impacket/tree/master)**)

  [![Python versions](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12-blue.svg)](https://github.com/fortra/impacket/tree/master)


Setup
=====

### Quick start

> :information_source: We recommend using `pipx` over `pip` for system-wide installations.

In order to grab the latest stable release run:

    python3 -m pipx install impacket

If you want to play with the unreleased changes, download the development 
version from the [master branch](https://github.com/fortra/impacket/tree/master),
extract the package, and execute the following command from the
directory where Impacket has been unpacked:

    python3 -m pipx install .

### Docker Support

Build Impacket's image:

      $ docker build -t "impacket:latest" .

Using Impacket's image:

      $ docker run -it --rm "impacket:latest"

Testing
=======

The library leverages the [pytest](https://docs.pytest.org/) framework for organizing
and marking test cases, [tox](https://tox.readthedocs.io/) to automate the process of
running them across supported Python versions, and [coverage](https://coverage.readthedocs.io/)
to obtain coverage statistics.

A [comprehensive testing guide](TESTING.md) is available.


Licensing
=========

This software is provided under a slightly modified version of
the Apache Software License. See the accompanying [LICENSE](LICENSE) file for
more information.

SMBv1 and NetBIOS support based on Pysmb by Michael Teo.

Disclaimer
==========

The spirit of this Open Source initiative is to help security researchers,
and the community, speed up research and educational activities related to
the implementation of networking protocols and stacks.

The information in this repository is for research and educational purposes
and not meant to be used in production environments and/or as part
of commercial products.

If you desire to use this code or some part of it for your own uses, we
recommend applying proper security development life cycle and secure coding
practices, as well as generate and track the respective indicators of
compromise according to your needs.


Contact Us
==========

Whether you want to report a bug, send a patch, or give some suggestions
on this package, reach out to us at https://www.coresecurity.com/about/contact.

For security-related questions check our [security policy](SECURITY.md).
