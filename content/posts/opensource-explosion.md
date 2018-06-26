---
title: "Collecting Exp during the Open Source Explosion"
date: 2018-05-29T09:13:58-05:00
---

## The Open Source Explosion ##

It is a pretty good time to be alive if you like tinkering with computer software.  There is a literal ton (I weighed it, just trust me) of free-to-use, open source software out there to take up your days, and help you accomplish crazy things, crazy efficiently.

As you can tell from my [resume](http://wbean1.info/resume.pdf), I make use of a lot of this software professionally:

* [ansible](https://www.ansible.com)
* [apache httpd](https://httpd.apache.org)
* [apache tomcat](https://tomcat.apache.org)
* [cloudfoundry](https://www.cloudfoundry.org)
* [collectd](https://collectd.org)
* [concourse](https://concourse-ci.org)
* [docker](https://www.docker.com)
* [elasticsearch](https://www.elastic.co/products/elasticsearch)
* [grafana](https://grafana.com)
* [haproxy](https://www.haproxy.org)
* [influxdb](https://portal.influxdata.com/downloads)
* [jenkins](https://jenkins.io)
* [kibana](https://www.elastic.co/products/kibana)
* [logstash](https://www.elastic.co/products/logstash)
* [memcached](https://memcached.org)
* [mysql](https://www.mysql.com) / [mariadb](https://mariadb.org)
* [nagios](https://www.nagios.org)
* [nginx](https://www.nginx.com)
* [packer](https://www.packer.io)
* [postgres](https://www.postgresql.org)
* [prometheus](https://prometheus.io)
* [puppet](https://puppet.com)
* [samba](https://www.samba.org)
* [sonarqube](https://sonarqube.org)
* [terraform](https://www.terraform.io)

But what makes an open source project *"good"*?  It all comes down to (in priority order):

1. **Useful** - the software must satisfy a need in an way that makes achieving some valuable result, easier.  Some of the value is in the result, some of the value is in the ease in which it is achieved.  Every single software I've listed above clears this primary hurdle exceptionally well, or it probably wouldn't be on this list.
2. **Well Documented** - the software must contain instructions that cover a majority of its functions or configurations.  In some cases, especially early in a software's lifecycle, industry adoption & discussions can fill in gaps here.  But for the long haul, people will git pissed if everything is hidden in tribal knowledge, discussions on internet forums, or deep in bug trackers.  And the software will lose adoption & thus potential contributors.
3. **Ease of Contribution** - the community surrounding the software makes contributing as frictionless as possible.  Most repos contain instructions on how to get started contributing to the project (setup local testing, etc...).  But there are other factors of frictionless contribution like... how complex is the surrounding ecosystem?, what are the personalities of the stewarding entities?, how "open" to change are the stewarding entities?

Delivering on all 3 of these attributes deserves a virtual High Five, and I'm constantly amazed there is so much software in such a good state.

## Gaining Exp ##

So you, like me, use a bunch of this software.  What can you do to transition from Corporate Leech towards an Altruistic Community Contributor?

Step #0 might be a battle to contribute.  Depending on your corporate culture, you might have to gain approval to sign "Contributor License Agreements", or forge inroads with your Legal team to make contributing back more frictionless.  Most of the time this is a simple conversation around why it makes business sense for software improvements to be upstreamed.  Do this.

Step #0.1 might be to join the dev-list / slack channel for the project and just be helpful.  If someone encounters a problem that you've seen before, [help them out](https://mail-archives.apache.org/mod_mbox/tomcat-users/201306.mbox/%3C1D613E56B17612448C6E50D9FD48A49307BF6C@EDXMB64.jdnet.deere.com%3E)!

Steps #1-thru-infinity: find small ways you can improve the software you use.  I am by no means an expert achiever in this area, but I have some [small](https://github.com/cloudfoundry-community/collectd-boshrelease/pull/16) [contributions](https://github.com/cloudfoundry/binary-builder/pull/17) to projects I care about.

Good software takes good people working goodly together.  The benefits to basically every industry and aspect of humanity's capabilities of open source software are staggering.  And kudos to the folks driving awesome projects openly.

[Some interesting open source hot-takes from the folks at github](https://blog.github.com/2018-02-08-open-source-project-trends-for-2018/)
