SOEMPIbin
=========

* Compiled binary distribution of [SOEMPI](http://github.com/MrCsabaToth/SOEMPI/) in an enterprise archive format, deployable to JBoss 4.2.3.GA-jdk6.
* For a more ready-to-use experience you can use this VirtualBox virtual machine http://hiplab.org/projects/soempi/bin/SOEMPIVM.7z
  * Compressed size: 583 MiB, uncompressed size: 2.1 GiB
  * Based on Ubuntu Linux 8.10 Server Interpid Ibex
  * username/pwd: ubuntu/reverse
  * Sun Java JDK 6
  * Contains PostgreSQL 8.3 with installed SOEMPI database schema (soempi/soempi)
  * JBoss 4.2.3-jdk6 with configured and deployed SOEMPI, located in /home/ububtu/jboss
  * When adding the VDI to the VirtualBox specify Am79C973 type emulated ethernet card
  * If you want the VM to see the internet select "Bridged Adapter" (see more in VirtualBox manuals)
  * In case you set up a multi-component SOEMPI scheme using more virtual machines you can separate them to an own subnet by selecting "Internal Network" (see more in VirtualBox manuals)
  * After boot-up and login, say "./jboss/bin/jboss start" from the home directory to start JBoss (and SOEMPI with it)
  * You can log-in to SOMEPI using the host computer's browser by visiting http://${VM_IPAddress}:8080/SOEMPI
  * You can see the JBoss console using the host computer's browser at http://${VM_IPAddress}:8080/
  * Stop the JBoss instance with "./jboss/bin/jboss stop"
