```
{
  "timestamp" : "2017-11-30T19:58:55.632Z",
  "clusters" : [ {
    "name" : "Rodo-dev",
    "version" : "CDH5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_enable_db_notification",
            "value" : "true"
          }, {
            "name" : "hive_metastore_java_heapsize",
            "value" : "1981808640"
          }, {
            "name" : "hive_metastore_server_max_message_size",
            "value" : "198180864"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_enable_impersonation",
            "value" : "false"
          }, {
            "name" : "hiveserver2_java_heapsize",
            "value" : "1981808640"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "3865470566"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "8453436211"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "409"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "1422"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "rodonode1.rodo.com"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "CapaCuatro1."
        }, {
          "name" : "hive_metastore_database_user",
          "value" : "cloudera"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "sentry_service",
          "value" : "sentry"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-18a2c14e9c8fe791df286c808e384369",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "b953184b-a955-4eb0-a789-738c410b93ea"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-7b8144d8841a58f0c9474c1d517d68a9",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "13ad938d-c969-4646-a92b-f4ae728c1206"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-bf454a659df03992cc83e171281f78c2",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-c2a9d0da4c85dfdf2c741b7b4f7817c9",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "49b2577f-1912-4373-8b0e-8db730295665"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-bf454a659df03992cc83e171281f78c2",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "c88ex9v1gnh8wj6159pk5n23u"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-bf454a659df03992cc83e171281f78c2",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1mp5gqyqjy583m1r1f914qw5"
          } ]
        }
      } ],
      "displayName" : "Hive"
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "enableSecurity",
          "value" : "true"
        } ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-18a2c14e9c8fe791df286c808e384369",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "b953184b-a955-4eb0-a789-738c410b93ea"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "e428y9007xchqj3secus80233"
          }, {
            "name" : "serverId",
            "value" : "2"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-7b8144d8841a58f0c9474c1d517d68a9",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "13ad938d-c969-4646-a92b-f4ae728c1206"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "591j7mzb5iqmqe3nay7t4xsu6"
          }, {
            "name" : "serverId",
            "value" : "3"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-bf454a659df03992cc83e171281f78c2",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dr43oxgrwde7x8jvdr2ifs2sf"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        }
      } ],
      "displayName" : "ZooKeeper"
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "database_host",
          "value" : "rodonode1.rodo.com"
        }, {
          "name" : "database_password",
          "value" : "CapaCuatro1."
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "database_user",
          "value" : "cloudera"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-HTTPFS-c2a9d0da4c85dfdf2c741b7b4f7817c9"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "sentry_service",
          "value" : "sentry"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_LOAD_BALANCER-bf454a659df03992cc83e171281f78c2",
        "type" : "HUE_LOAD_BALANCER",
        "hostRef" : {
          "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7uhvul1bc3025pzbr68b3gxy2"
          } ]
        }
      }, {
        "name" : "hue-HUE_SERVER-bf454a659df03992cc83e171281f78c2",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
        },
        "config" : {
          "items" : [ {
            "name" : "navmetadataserver_cmdb_password",
            "value" : "6d792cfd-9959-41a7-a350-80f8eac2c7b7"
          }, {
            "name" : "role_jceks_password",
            "value" : "63clttrefblz8aq9rc7d3pyxa"
          }, {
            "name" : "secret_key",
            "value" : "Xp7K6zLeb7UJdUyJhfRHqAAm9UsW2W"
          } ]
        }
      }, {
        "name" : "hue-KT_RENEWER-bf454a659df03992cc83e171281f78c2",
        "type" : "KT_RENEWER",
        "hostRef" : {
          "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5y3eb25y0mdq47dwhhf2j1txo"
          } ]
        }
      } ],
      "displayName" : "Hue"
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "OOZIE_SERVER",
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "rodonode1.rodo.com"
          }, {
            "name" : "oozie_database_password",
            "value" : "CapaCuatro1."
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "cloudera"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-bf454a659df03992cc83e171281f78c2",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "czhkq8fmcwabnksqb3teuy4sr"
          } ]
        }
      } ],
      "displayName" : "Oozie"
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "12"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "3"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "container_executor_min_user_id",
            "value" : "0"
          }, {
            "name" : "rm_cpu_shares",
            "value" : "1600"
          }, {
            "name" : "rm_io_weight",
            "value" : "800"
          }, {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/mnt/resource/yarn/nm,/opt/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/mnt/resource/yarn/container-logs,/opt/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "6"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "14162"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "18616"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "6"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "80"
        }, {
          "name" : "yarn_service_cgroups",
          "value" : "false"
        }, {
          "name" : "yarn_service_lce_always",
          "value" : "false"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "Cdeu0VD3xcIUsl7rUDkoSnE0ouIWMF"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-bf454a659df03992cc83e171281f78c2",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6esehl6bv30gui6lmlfvg0u4p"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-18a2c14e9c8fe791df286c808e384369",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "b953184b-a955-4eb0-a789-738c410b93ea"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8te1p5jh4qtj2f8v6n3y30cmp"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-7b8144d8841a58f0c9474c1d517d68a9",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "13ad938d-c969-4646-a92b-f4ae728c1206"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "cy5c7qrk6jd3qtkum3snl7mce"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-c2a9d0da4c85dfdf2c741b7b4f7817c9",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "49b2577f-1912-4373-8b0e-8db730295665"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "13xh4e1tnc1supbupxyjwhkqt"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-bf454a659df03992cc83e171281f78c2",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "46"
          }, {
            "name" : "role_jceks_password",
            "value" : "3ibf8obkz563u0velzbn3w37m"
          } ]
        }
      } ],
      "displayName" : "YARN (MR2 Included)"
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "datanode_java_heapsize",
            "value" : "1073741824"
          }, {
            "name" : "dfs_data_dir_list",
            "value" : "/mnt/resource/dfs/dn,/opt/dfs/dn"
          }, {
            "name" : "dfs_datanode_data_dir_perm",
            "value" : "700"
          }, {
            "name" : "dfs_datanode_failed_volumes_tolerated",
            "value" : "1"
          }, {
            "name" : "dfs_datanode_http_port",
            "value" : "1006"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4315938816"
          }, {
            "name" : "dfs_datanode_port",
            "value" : "1004"
          }, {
            "name" : "rm_cpu_shares",
            "value" : "400"
          }, {
            "name" : "rm_io_weight",
            "value" : "200"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "JOURNALNODE",
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/opt/journalnodes"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/disk4/dfs/nn,/mnt/resource/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          }, {
            "name" : "namenode_java_heapsize",
            "value" : "1981808640"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/disk4/dfs/snn"
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "1981808640"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_encrypt_data_transfer_algorithm",
          "value" : "AES/CTR/NoPadding"
        }, {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "KUAMRlh9ESFF02GULdd8QsHjHn3gl6"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "fLH9V4zAoL4q8tj2IX6ZeKsdbnW0Gv"
        }, {
          "name" : "hadoop_security_authentication",
          "value" : "kerberos"
        }, {
          "name" : "hadoop_security_authorization",
          "value" : "true"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "Y82CWVC3VdMKxtZ1YwpCt5v0mfQjCj"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "20"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-bf454a659df03992cc83e171281f78c2",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-18a2c14e9c8fe791df286c808e384369",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "b953184b-a955-4eb0-a789-738c410b93ea"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "63xc1cftxbe2khoxlc377ltdb"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-7b8144d8841a58f0c9474c1d517d68a9",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "13ad938d-c969-4646-a92b-f4ae728c1206"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "cmqqk2jltn4it95kjqxzmodir"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-c2a9d0da4c85dfdf2c741b7b4f7817c9",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "49b2577f-1912-4373-8b0e-8db730295665"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "et9sv7jrh0zbeux681ukt5cir"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-7b8144d8841a58f0c9474c1d517d68a9",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "13ad938d-c969-4646-a92b-f4ae728c1206"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "31h2d1dvq4im7yd6u86l1k7zm"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-bf454a659df03992cc83e171281f78c2",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "45bh8kyhzj9u6n72wcj145vnv"
          } ]
        }
      }, {
        "name" : "hdfs-HTTPFS-c2a9d0da4c85dfdf2c741b7b4f7817c9",
        "type" : "HTTPFS",
        "hostRef" : {
          "hostId" : "49b2577f-1912-4373-8b0e-8db730295665"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8tgo7ylxyykveuuqwyvz6m49f"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-18a2c14e9c8fe791df286c808e384369",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "b953184b-a955-4eb0-a789-738c410b93ea"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "cc9i6fbv1ekvcow24pad181o0"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-7b8144d8841a58f0c9474c1d517d68a9",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "13ad938d-c969-4646-a92b-f4ae728c1206"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "b58jxghs5ughj3pb59hfqumbk"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-bf454a659df03992cc83e171281f78c2",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "d8p83p22ionwzxxe75k8tp451"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-7b8144d8841a58f0c9474c1d517d68a9",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "13ad938d-c969-4646-a92b-f4ae728c1206"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "55"
          }, {
            "name" : "role_jceks_password",
            "value" : "4v1x44ltwzj7y7rkbegw8jygl"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-bf454a659df03992cc83e171281f78c2",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "48"
          }, {
            "name" : "role_jceks_password",
            "value" : "d6ys2jw3spzjwwzw8db9j009d"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    }, {
      "name" : "sentry",
      "type" : "SENTRY",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "SENTRY_SERVER",
          "items" : [ {
            "name" : "sentry_server_java_heapsize",
            "value" : "970981376"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "sentry_server_database_host",
          "value" : "rodonode1.rodo.com"
        }, {
          "name" : "sentry_server_database_password",
          "value" : "CapaCuatro1."
        }, {
          "name" : "sentry_server_database_user",
          "value" : "cloudera"
        }, {
          "name" : "sentry_service_admin_group",
          "value" : "hive,impala,hue,solr,kafka,rodo"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "sentry-SENTRY_SERVER-bf454a659df03992cc83e171281f78c2",
        "type" : "SENTRY_SERVER",
        "hostRef" : {
          "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dfg6pcd3bpbj4gem5tbsc7bv5"
          } ]
        }
      } ],
      "displayName" : "Sentry"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9",
    "ipAddress" : "10.2.0.4",
    "hostname" : "rodonode1.rodo.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "13ad938d-c969-4646-a92b-f4ae728c1206",
    "ipAddress" : "10.2.0.5",
    "hostname" : "rodonode2.rodo.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "b953184b-a955-4eb0-a789-738c410b93ea",
    "ipAddress" : "10.2.0.6",
    "hostname" : "rodonode3.rodo.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "49b2577f-1912-4373-8b0e-8db730295665",
    "ipAddress" : "10.2.0.7",
    "hostname" : "rodonode4.rodo.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__hue-HUE_SERVER-bf454a659df03992cc83e171281f78c2",
    "roles" : [ "ROLE_NAVIGATOR_ADMIN" ],
    "pwHash" : "04d7fd6dacb459815173e14f4002a9ce24593c3ae57761be44636d319bdc728d",
    "pwSalt" : 6825505070027398359,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-bf454a659df03992cc83e171281f78c2",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "1cadbd77e507d28d215b81f91b60db8c141bd890cc2ee654596ad55336c216ca",
    "pwSalt" : -305331612900773598,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-bf454a659df03992cc83e171281f78c2",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "b34600874b5267d680179c78aeb51798bac64ffd2205202b57be7864479fcc0d",
    "pwSalt" : 4632885490071015572,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-bf454a659df03992cc83e171281f78c2",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "87f49a5ac323d955e00c147d7232f5d52d614b02547494cbddbaff6096975002",
    "pwSalt" : -4498365708074278127,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-bf454a659df03992cc83e171281f78c2",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "2263144f89b1529783387d0538614f7b673d9127abbbc282d25aee611f91adbc",
    "pwSalt" : 5572721426986877034,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ],
    "pwHash" : "09305d61772dacfd3587b7fa03bb6540bec9daabd1159f66b75115b461eab94e",
    "pwSalt" : -8978159349190366759,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "3e5b6d762e33e2dd45783f5e94fd950e4831e95bec9e788b5b13b67c08c8f792",
    "pwSalt" : -7388333381936339232,
    "pwLogin" : true
  }, {
    "name" : "rodo-dev",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "802ba946ec13a68122a2d264dd66269e77ffd6f6a090832740150b06823a0d38",
    "pwSalt" : 4004637330207273047,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.13.0",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20171002-1719",
    "gitHash" : "bd657e597e6743c458ee2c9aabe808b7c972981c",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "CapaCuatro1."
        }, {
          "name" : "headlamp_database_user",
          "value" : "cloudera"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-bf454a659df03992cc83e171281f78c2",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "e4xg0vab6ff682422jkw6622t"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-bf454a659df03992cc83e171281f78c2",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "9a1930k407sxs222d71otn9r7"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-bf454a659df03992cc83e171281f78c2",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "6nmzaaf811mh0uvsczoa75djt"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-bf454a659df03992cc83e171281f78c2",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "d0zzj94xt4bm8mleoy89ng9jv"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-bf454a659df03992cc83e171281f78c2",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "2b2ec2cd-586f-4fda-a90e-e3078ed64fa9"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "aeun2f06gg4792roii4qdxrls"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "AD_USE_SIMPLE_AUTH",
      "value" : "false"
    }, {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/25/2012 4:30"
    }, {
      "name" : "KDC_ADMIN_HOST",
      "value" : "rodonode1.rodo.com"
    }, {
      "name" : "KDC_ADMIN_PASSWORD",
      "value" : "BQIAAAA7AAEACFJPRE8uQ09NAAxjbG91ZGVyYS1zY20AAAABWh8uRwEAFwAQ6Jf8GFkO8iQ3Th9kv9hVtQAAAAE="
    }, {
      "name" : "KDC_ADMIN_USER",
      "value" : "cloudera-scm@RODO.COM"
    }, {
      "name" : "KDC_HOST",
      "value" : "rodonode1.rodo.com"
    }, {
      "name" : "KRB_ENC_TYPES",
      "value" : "arcfour-hmac"
    }, {
      "name" : "KRB_MANAGE_KRB5_CONF",
      "value" : "true"
    }, {
      "name" : "MAX_RENEW_LIFE",
      "value" : "604800"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "NOT_ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,http://archive.cloudera.com/kudu/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
    }, {
      "name" : "SECURITY_REALM",
      "value" : "RODO.COM"
    } ]
  }
  
