There are 3 modes in installation in Hadoop.
  1. Local (Standalone) Mode
  2. Pseudo-Distributed Mode
  3. Fully-Distributed Mode

Basic requirements for installing hadoop 1.x is:
  1. Nix Operating system i.e linux or unix operating systems
  2. Java 1.7 or later
  3. SSH (Secure Shell)

## Local Mode ##
* In this mode it will act as a simple Java Program.
* To run Hadoop in Local Mode, set the JAVA_HOME environment variable in hadoop/conf/hadoop-env.sh
* None of the Hadoop deamons will be running in this mode.
* Do the following changes in ~/.bashrc file.
```
  export JAVA_HOME=/usr/local/jdk1.7.0_71
  export PATH=$PATH:$JAVA_HOME/bin 
```
and now apply changes into the current system
```
  $source ~/.bashrc
```
* Do the following change in hadoop-env.sh

  `export JAVA_HOME=/path/to/java_home`

## Pseudo-Distributed Mode ##
* In this mode all the hadoop deamons will be running in a single machine.
* To install Hadoop in Pseudo-Distributed Mode, we need to change the following files:
```
  1. hadoop-env.sh
  2. core-site.xml
  3. hdfs-site.xml
  4. mapred-site.xml
  5. masters
  6. slaves
```
