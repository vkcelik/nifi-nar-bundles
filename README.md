The NAR files with the longer version numbers in the file name (e.g. 'nifi-jms-processors-nar-1.1.0.2.1.2.0-10.nar') are original non-patched NAR files from HDF NiFi. These files do not have support for IBM MQ multi-instance queue managers 

The NAR files with the shorter version numbers in the file name (e.g. 'nifi-jms-processors-nar-1.1.0.nar') are improved NAR files compiled from the official Apache NiFi releases. These NAR files have support for IBM MQ multi-instance queue managers

Compilation:
- cd nifi-nar-bundles\nifi-jms-bundle
- mvn clean package -Dmaven.test.skip=true -pl nifi-jms-processors-nar -am
OR 
- mvn clean package -pl nifi-jms-processors-nar -am