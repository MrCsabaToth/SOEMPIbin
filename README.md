SOEMPIbin
=========

* Compiled binary distribution of [SOEMPI](http://github.com/MrCsabaToth/SOEMPI/) in an enterprise archive format, deployable to JBoss 4.2.3.GA-jdk6.
* For a more ready-to-use experience you can use this [VirtualBox virtual machine](http://hiplab.org/projects/soempi/bin/SOEMPIVM.7z) (compressed with 7Zip)
  * OVA format portable image exported from VirtualBox
  * Compressed size: 1.2 GiB, uncompressed size: 1.5 GiB
  * Based on Ubuntu Linux 8.10 Server Interpid Ibex
  * username/pwd: ubuntu/reverse
  * Sun Java JDK 6
  * Contains PostgreSQL 8.3 with installed SOEMPI database schema (soempi/soempi)
  * JBoss 4.2.3-jdk6 with configured and deployed SOEMPI, located in /home/ububtu/jboss
  * After boot-up and login, say "sudo ./jboss/bin/jboss start" from the home directory to start JBoss (and SOEMPI with it)
  * You can log-in to SOMEPI using the host computer's browser by visiting http://${VM_IPAddress}:8080/SOEMPI
  * You can see the JBoss console using the host computer's browser at http://${VM_IPAddress}:8080/
  * You can connect to the PostgreSQL database on the VM's 5432 port (standard PostgreSQL port)
  * Stop the JBoss instance with "sudo ./jboss/bin/jboss stop"
  * Note, that nor the JBoss nor the PostgreSQL is hardened, this VM is for demonstration purposes
