MapR Client Install Instructions
================================
Install MapR client on your Mac/Windows client system by following instructions given at the link.
Follow instructions at http://maprdocs.mapr.com/home/AdvancedInstallation/SettingUptheClient-install-mapr-client.html

IDE Configurations
===================
For running application from IDE add one of the following to your run configurations.

1. Add VM options flag as "-Dfs.mapr.bailout.on.library.mismatch=false" OR

2. Add Environment variable "DISABLE_LIB_MISMATCH" with "true" value.

Running from Command line
===========

Build the project using:

    mvn clean install

Run following command to execute OJAI_002_GetStoreAndInsertDocuments class:

    java -cp $(mapr classpath):target/ojai-2-samples-1.0-SNAPSHOT.jar com.mapr.ojai.examples.OJAI_002_GetStoreAndInsertDocuments
