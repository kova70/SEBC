CM Monitoring Lab

What is ubertask optimization?
Whether to enable the small-jobs "ubertask" optimization, which runs "sufficiently small" jobs sequentially within a single JVM. "Small" is defined by the following maxmaps, maxreduces, and maxbytes settings. Note that configurations for application masters also affect the "Small" definition - yarn.app.mapreduce.am.resource.mb must be larger than both mapreduce.map.memory.mb and mapreduce.reduce.memory.mb, and yarn.app.mapreduce.am.resource.cpu-vcores must be larger than both mapreduce.map.cpu.vcores and mapreduce.reduce.cpu.vcores to enable ubertask. Users may override this value. 
Source:https://archive.cloudera.com/cdh5/cdh/5/hadoop/hadoop-mapreduce-client/hadoop-mapreduce-client-core/mapred-default.xml

Where in CM is the Kerberos Security Realm value displayed?
Dentro de Administración -> Seguridad -> Credenciales Kerberos -> Configuracion 
Dominio de seguridad de Kerberos (default_realm)
Link, para mi laboratorio:http://rodonode1.cloudapp.net:7180/cmf/settings?groupKey=config.common.kerberos.display_group&groupParent=#filtercategory=Ajustes&filterdisplayGroup=Kerberos&filterfreeText=key

Which CDH service(s) host a property for enabling Kerberos authentication?
HDFS service
FLUME
HBASE
Hive
HUE 
IMPALA
OOZIE
SOLR
SPARK
ZooKeeper.
HDFS HTTP Web-Consoles Note: This is effective only if Kerberos is enabled for the HDFS service.

How do you upgrade the CM agents?

To manually upgrade the Cloudera Manager agent:
On all cluster hosts except the Cloudera Manager Server host, stop the Agent:
sudo service cloudera-scm-agent stop
Select No, I would like to skip the agent upgrade now and click Continue.
Copy the repo file 
Run the following commands on all hosts except the Cloudera Manager Server host:
RHEL
    sudo yum clean all
    sudo yum upgrade cloudera-manager-daemons cloudera-manager-agent

Cloudera Manager upgrades Agent software

    When Cloudera Manager upgrades the Cloudera Manager agent, Cloudera Manager handles the upgrade and cleanup, and optionally upgrades the JDK.
        Select Yes, I would like to upgrade the Cloudera Manager Agent packages now and click Continue.
        Select the release of the Cloudera Manager Agent to install. Normally, this is the Matched Release for this Cloudera Manager Server. However, if you used a custom repository (instead of archive.cloudera.com) for the Cloudera Manager server, select Custom Repository and provide the required information. The custom repository location must contain the matched Agent version. See Creating and Using a Package Repository for Cloudera Manager. Custom repositories are required when your cluster cannot access the Internet, or when you need to upgrade to a version other that the most current version of Cloudera Manager.
        Click Continue. The JDK Installation Options page displays.
            If you want Cloudera Manager to install JDK 1.7 on all cluster hosts, select Install Oracle Java SE Development Kit (JDK) .
            If local laws permit you to deploy unlimited strength encryption, and you are running a secure cluster, select the Install Java Unlimited Strength Encryption Policy Files checkbox.
        Click Continue.
        Specify credentials and initiate Agent installation:
            Select root or enter the username for an account that has password-less sudo permission.
            Select an authentication method:
                If you choose password authentication, enter and confirm the password.
                If you choose public-key authentication, provide a passphrase and path to the required key files.
            You can specify an alternate SSH port. The default value is 22.
            You can specify the maximum number of host installations to run at once. The default value is 10.
        Click Continue.
        The Cloudera Manager Agent packages and, if selected, the JDK are installed.
        Click Continue.
        The Host Inspector runs to inspect your managed hosts for correct versions and configurations. If problems occur, you can make changes and then rerun the inspector.
        When you are satisfied with the inspection results, click Continue.

Give the tsquery statement used to chart Hue's CPU utilization?
  select cpu_user_rate where roleType=HUE_SERVER
  
Name all the roles that make up the Hive service
    HIVE:
      Hive Metastore Server
      HiveServer2
      
What steps must be completed before integrating Cloudera Manager with Kerberos?
  1 - Configuration of DNS and Reverse DNS Resolutions
  2 - Configuration of MIT KDC or another KDC  ( Server configurations )
  3 - Create a user with administrative privileges on KDC Server ( cloudera-scm user for example (addprinc cloudera-scm@REALM.CORP) )
  4 - Install the krb5-libs and krb5-workstation and openldap-clients on every node
  5 - Install or upgrade the Java JCE Polices ( for provide authentication with AES-256 (aes256-cts-hmac-sha1-96) )
  6 - Configure /etc/krb5.conf for every node
  7 - Make a test to verify if the firewall is allow ports 88 TCP/UDP, 464 TCP/UDP, 749 TCP, 754 TCP for every node
  8 - Configure the minimum user id ( to 500 or less then, it's depends of the KDC are you using.. MIT KDC, MSAD, RED HAT IDM... N)
  
