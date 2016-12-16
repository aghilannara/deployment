This repository contains ansible roles for setting up HDP cluster

Coverage of this ansible role repository is to cover:

* setting up java in all nodes
* setting up SSH key in all nodes
* setting up ambari in a single ambari node
* setting up repository mirror

===================
Available Roles
===================

abyres.hdpnode
================

Purpose: Setup the basic requirements on a server before it can be used as a
HDP node. 

Tasks:

* disable selinux
* install hdp repository
* install oracle java 1.7
* setup oracle java as default system java
* install SSH key

abyres.ambari-server
===================

Purpose: Setup ambari server 

Tasks:

abyres.hdp-mirror
================

Purpose: Setup HDP mirror for faster local installation

Tasks:

abyres.hdp-pgsql
================

Purpose: Setup remote Postgresql to be used as ambari server metadata

Tasks:

abyres.ntpd
===========

Purpose: Setup ntpd

Tasks:

abyres.dnsmasq
==============

Purpose: Setup dnsmasq

Tasks:

abyres.libvirtd
===============

Purpose: Setup libvirtd

Tasks:

abyres.resolv
=============

Purpose: Configure /etc/resolve 

Tasks:

abyres.hdf-ambari-server
=======================

Purpose: setup HDF cluster (must be separate IP thab HDP cluster!)

Tasks: install HDF cluster, set up ambari-server with mpack setup.

abyres.java_version
======================

purpose: install latest java version specified in playbook.yml.sample with localrepo connected

Tasks: ensure latest java is applied all over in clusters
