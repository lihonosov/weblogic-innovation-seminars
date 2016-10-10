### Introduction ###

#### Domain to Partition Conversion tool ####
The Domain to Partition Conversion Tool (DPCT) provides a utility that inspects a specified source domain and produces an archive containing the resources, deployed applications and other settings.  This can then be used with the Import Partition operation provided in WebLogic Server 12.2.1 to create a new partition that represents the original source domain.  An external overrides file is generated (in JSON format) that can be modified to adjust the targets and names used for the relevant artifacts when they are created in the partition. DPCT supports WebLogic Server 10.3.6, 12.1.1, 12.1.2 and 12.1.3 source domains and makes the conversion to WebLogic Server 12.2.1 partitions a straightforward process.

#### Lift and shift ####
During our labs we show how to move existing domain partition running in On-Premise WebLogic Server by export and import capabilities to WebLogic Server running inside Java Cloud Service. We prepared single maven command that copy domain partition files in to Java Cloud Service VM as well as copy and execute all SQL files on DataBase Cloud Service environment to create working environment for our lab. In this HOL we keep domain and database configuration simple.

----

### Prerequisites ###

This lab require to build the model of on-premise enviornment. See [Preparation of the on-premise environment](https://github.com/oracle-weblogic/weblogic-innovation-seminars/blob/caf-12.2.1/cloud.demos/jcs.basics/vbox.vm.md)