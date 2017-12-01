* List the cloud provider you are using
    * AZURE
* List your instances by IP address and DNS name
    * nodo1.westus.cloudapp.azure.com       40.112.220.46 
    * nodo2.westus.cloudapp.azure.com       104.209.38.190 
    * nodo3.westus.cloudapp.azure.com       104.209.33.1 
    * nodo4.westus.cloudapp.azure.com        13.64.145.151 
* List the Linux release you are using
     * `hostnamectl`
       * Static hostname: nodo1
       * Icon name: computer-vm
       * Chassis: vm
       * Machine ID: cb569fbd0b8a4acdaec9183b444c5718
       * Boot ID: c0b225ab405e47d58abc3f607abf4c78
       * Virtualization: microsoft
       * Operating System: Red Hat Enterprise Linux Server 7.4 (Maipo)
       * CPE OS Name: cpe:/o:redhat:enterprise_linux:7.4:GA:server
       * Kernel: Linux 3.10.0-693.11.1.el7.x86_64
       * Architecture: x86-64
* List the file system capacity for the first node
     * `df -h`
        * Filesystem      Size  Used Avail Use% Mounted on
        * /dev/sda2        32G  1.2G   31G   4% /
        * devtmpfs         16G     0   16G   0% /dev
        * tmpfs            16G     0   16G   0% /dev/shm
        * tmpfs            16G  8.4M   16G   1% /run
        * tmpfs            16G     0   16G   0% /sys/fs/cgroup
        * /dev/sdc1        80G   33M   80G   1% /opt
        * /dev/sda1       497M  129M  368M  26% /boot
        * /dev/sdb1        63G  2.1G   58G   4% /mnt/resource
        * tmpfs           3.2G     0  3.2G   0% /run/user/1000
* List the command and output for yum repolist enabled
     * `yum repolist enabled`<br>
        Loaded plugins: langpacks, product-id, search-disabled-repos
        rhui-microsoft-azure-rhel7                                                                                                                                                 | 2.9 kB  00:00:00     
        rhui-rhel-7-server-dotnet-rhui-debug-rpms                                                                                                                                  | 3.8 kB  00:00:00     
        rhui-rhel-7-server-dotnet-rhui-rpms                                                                                                                                        | 4.0 kB  00:00:00     
        rhui-rhel-7-server-dotnet-rhui-source-rpms                                                                                                                                 | 3.8 kB  00:00:00     
        rhui-rhel-7-server-rhui-debug-rpms                                                                                                                                         | 3.3 kB  00:00:00     
        rhui-rhel-7-server-rhui-extras-debug-rpms                                                                                                                                  | 3.2 kB  00:00:00     
        rhui-rhel-7-server-rhui-extras-rpms                                                                                                                                        | 3.4 kB  00:00:00     
        rhui-rhel-7-server-rhui-extras-source-rpms                                                                                                                                 | 3.8 kB  00:00:00     
        rhui-rhel-7-server-rhui-optional-debug-rpms                                                                                                                                | 3.3 kB  00:00:00     
        rhui-rhel-7-server-rhui-optional-rpms                                                                                                                                      | 3.5 kB  00:00:00     
        rhui-rhel-7-server-rhui-optional-source-rpms                                                                                                                               | 3.8 kB  00:00:00     
        rhui-rhel-7-server-rhui-rh-common-debug-rpms                                                                                                                               | 3.8 kB  00:00:00     
        rhui-rhel-7-server-rhui-rh-common-rpms                                                                                                                                     | 3.8 kB  00:00:00     
        rhui-rhel-7-server-rhui-rh-common-source-rpms                                                                                                                              | 3.8 kB  00:00:00     
        rhui-rhel-7-server-rhui-rpms                                                                                                                                               | 3.5 kB  00:00:00     
        rhui-rhel-7-server-rhui-source-rpms                                                                                                                                        | 3.8 kB  00:00:00     
        rhui-rhel-7-server-rhui-supplementary-debug-rpms                                                                                                                           | 3.7 kB  00:00:00     
        rhui-rhel-7-server-rhui-supplementary-rpms                                                                                                                                 | 3.4 kB  00:00:00     
        rhui-rhel-7-server-rhui-supplementary-source-rpms                                                                                                                          | 3.8 kB  00:00:00     
        rhui-rhel-server-rhui-rhscl-7-debug-rpms                                                                                                                                   | 3.4 kB  00:00:00     
        rhui-rhel-server-rhui-rhscl-7-rpms                                                                                                                                         | 3.5 kB  00:00:00     
        rhui-rhel-server-rhui-rhscl-7-source-rpms                                                                                                                                  | 3.8 kB  00:00:00     
        (1/64): rhui-rhel-7-server-dotnet-rhui-debug-rpms/7Server/x86_64/group                                                                                                     |  104 B  00:00:00     
        (2/64): rhui-rhel-7-server-dotnet-rhui-debug-rpms/7Server/x86_64/primary_db                                                                                                |  17 kB  00:00:00     
        (3/64): rhui-microsoft-azure-rhel7/primary_db                                                                                                                              | 2.3 kB  00:00:00     
        (4/64): rhui-rhel-7-server-dotnet-rhui-rpms/7Server/x86_64/updateinfo                                                                                                      |  11 kB  00:00:00     
        (5/64): rhui-rhel-7-server-dotnet-rhui-debug-rpms/7Server/x86_64/updateinfo                                                                                                | 4.5 kB  00:00:00     
        (6/64): rhui-rhel-7-server-dotnet-rhui-source-rpms/7Server/x86_64/group                                                                                                    |  104 B  00:00:00     
        (7/64): rhui-rhel-7-server-dotnet-rhui-rpms/7Server/x86_64/primary_db                                                                                                      |  48 kB  00:00:00     
        (8/64): rhui-rhel-7-server-dotnet-rhui-rpms/7Server/x86_64/group                                                                                                           |  104 B  00:00:00     
        (9/64): rhui-rhel-7-server-dotnet-rhui-source-rpms/7Server/x86_64/updateinfo                                                                                               | 4.9 kB  00:00:00     
        (10/64): rhui-rhel-7-server-rhui-debug-rpms/7Server/x86_64/group                                                                                                           |  104 B  00:00:00     
        (11/64): rhui-rhel-7-server-rhui-extras-debug-rpms/x86_64/group                                                                                                            |  104 B  00:00:00     
        (12/64): rhui-rhel-7-server-rhui-extras-debug-rpms/x86_64/updateinfo                                                                                                       |  77 kB  00:00:00     
        (13/64): rhui-rhel-7-server-rhui-debug-rpms/7Server/x86_64/primary_db                                                                                                      | 2.8 MB  00:00:00     
        (14/64): rhui-rhel-7-server-rhui-extras-debug-rpms/x86_64/primary_db                                                                                                       |  30 kB  00:00:00     
        (15/64): rhui-rhel-7-server-dotnet-rhui-source-rpms/7Server/x86_64/primary_db                                                                                              |  14 kB  00:00:00     
        (16/64): rhui-rhel-7-server-rhui-extras-rpms/x86_64/group                                                                                                                  |  104 B  00:00:00     
        (17/64): rhui-rhel-7-server-rhui-extras-source-rpms/x86_64/group                                                                                                           |  104 B  00:00:00     
        (18/64): rhui-rhel-7-server-rhui-extras-rpms/x86_64/primary_db                                                                                                             | 326 kB  00:00:00     
        (19/64): rhui-rhel-7-server-rhui-extras-source-rpms/x86_64/updateinfo                                                                                                      | 143 kB  00:00:00     
        (20/64): rhui-rhel-7-server-rhui-debug-rpms/7Server/x86_64/updateinfo                                                                                                      | 1.6 MB  00:00:00     
        (21/64): rhui-rhel-7-server-rhui-extras-source-rpms/x86_64/primary_db                                                                                                      |  83 kB  00:00:00     
        (22/64): rhui-rhel-7-server-rhui-optional-debug-rpms/7Server/x86_64/updateinfo                                                                                             | 1.2 MB  00:00:00     
        (23/64): rhui-rhel-7-server-rhui-extras-rpms/x86_64/updateinfo                                                                                                             | 222 kB  00:00:00     
        (24/64): rhui-rhel-7-server-rhui-optional-rpms/7Server/x86_64/group                                                                                                        |  24 kB  00:00:00     
        (25/64): rhui-rhel-7-server-rhui-optional-debug-rpms/7Server/x86_64/primary_db                                                                                             | 2.1 MB  00:00:00     
        (26/64): rhui-rhel-7-server-rhui-optional-rpms/7Server/x86_64/updateinfo                                                                                                   | 1.7 MB  00:00:00     
        (27/64): rhui-rhel-7-server-rhui-optional-debug-rpms/7Server/x86_64/group                                                                                                  |  104 B  00:00:00     
        (28/64): rhui-rhel-7-server-rhui-optional-source-rpms/7Server/x86_64/group                                                                                                 |  104 B  00:00:00     
        (29/64): rhui-rhel-7-server-rhui-rh-common-debug-rpms/7Server/x86_64/group                                                                                                 |  104 B  00:00:00     
        (30/64): rhui-rhel-7-server-rhui-rh-common-debug-rpms/7Server/x86_64/updateinfo                                                                                            |  11 kB  00:00:00     
        (31/64): rhui-rhel-7-server-rhui-optional-source-rpms/7Server/x86_64/primary_db                                                                                            | 1.3 MB  00:00:00     
        (32/64): rhui-rhel-7-server-rhui-rh-common-debug-rpms/7Server/x86_64/primary_db                                                                                            |  12 kB  00:00:00     
        (33/64): rhui-rhel-7-server-rhui-rh-common-rpms/7Server/x86_64/group                                                                                                       |  104 B  00:00:00     
        (34/64): rhui-rhel-7-server-rhui-optional-source-rpms/7Server/x86_64/updateinfo                                                                                            | 236 kB  00:00:00     
        (35/64): rhui-rhel-7-server-rhui-optional-rpms/7Server/x86_64/primary_db                                                                                                   | 6.1 MB  00:00:00     
        (36/64): rhui-rhel-7-server-rhui-rh-common-rpms/7Server/x86_64/primary_db                                                                                                  | 119 kB  00:00:00     
        (37/64): rhui-rhel-7-server-rhui-rh-common-source-rpms/7Server/x86_64/group                                                                                                |  104 B  00:00:00     
        (38/64): rhui-rhel-7-server-rhui-rh-common-source-rpms/7Server/x86_64/updateinfo                                                                                           |  24 kB  00:00:00     
        (39/64): rhui-rhel-7-server-rhui-rh-common-source-rpms/7Server/x86_64/primary_db                                                                                           |  34 kB  00:00:00     
        (40/64): rhui-rhel-7-server-rhui-rh-common-rpms/7Server/x86_64/updateinfo                                                                                                  |  32 kB  00:00:00     
        (41/64): rhui-rhel-7-server-rhui-source-rpms/7Server/x86_64/group                                                                                                          |  104 B  00:00:00     
        (42/64): rhui-rhel-7-server-rhui-rpms/7Server/x86_64/updateinfo                                                                                                            | 2.4 MB  00:00:00     
        (43/64): rhui-rhel-7-server-rhui-supplementary-debug-rpms/7Server/x86_64/group                                                                                             |  104 B  00:00:00     
        (44/64): rhui-rhel-7-server-rhui-source-rpms/7Server/x86_64/updateinfo                                                                                                     | 1.7 MB  00:00:00     
        (45/64): rhui-rhel-7-server-rhui-source-rpms/7Server/x86_64/primary_db                                                                                                     | 2.1 MB  00:00:00     
        (46/64): rhui-rhel-7-server-rhui-supplementary-debug-rpms/7Server/x86_64/updateinfo                                                                                        |   76 B  00:00:00     
        (47/64): rhui-rhel-7-server-rhui-rpms/7Server/x86_64/group                                                                                                                 | 709 kB  00:00:00     
        (48/64): rhui-rhel-7-server-rhui-supplementary-debug-rpms/7Server/x86_64/primary_db                                                                                        | 1.5 kB  00:00:00     
        (49/64): rhui-rhel-7-server-rhui-supplementary-rpms/7Server/x86_64/group                                                                                                   |  40 kB  00:00:00     
        (50/64): rhui-rhel-7-server-rhui-supplementary-rpms/7Server/x86_64/updateinfo                                                                                              |  55 kB  00:00:00     
        (51/64): rhui-rhel-7-server-rhui-supplementary-rpms/7Server/x86_64/primary_db                                                                                              | 262 kB  00:00:00     
        (52/64): rhui-rhel-7-server-rhui-supplementary-source-rpms/7Server/x86_64/group                                                                                            |  104 B  00:00:00     
        (53/64): rhui-rhel-7-server-rhui-supplementary-source-rpms/7Server/x86_64/updateinfo                                                                                       | 9.5 kB  00:00:00     
        (54/64): rhui-rhel-server-rhui-rhscl-7-debug-rpms/7Server/x86_64/group                                                                                                     |  104 B  00:00:00     
        (55/64): rhui-rhel-server-rhui-rhscl-7-debug-rpms/7Server/x86_64/updateinfo                                                                                                | 222 kB  00:00:00     
        (56/64): rhui-rhel-server-rhui-rhscl-7-debug-rpms/7Server/x86_64/primary_db                                                                                                | 231 kB  00:00:00     
        (57/64): rhui-rhel-server-rhui-rhscl-7-rpms/7Server/x86_64/group                                                                                                           |  104 B  00:00:00     
        (58/64): rhui-rhel-server-rhui-rhscl-7-rpms/7Server/x86_64/updateinfo                                                                                                      | 860 kB  00:00:00     
        (59/64): rhui-rhel-7-server-rhui-rpms/7Server/x86_64/primary_db                                                                                                            |  45 MB  00:00:00     
        (60/64): rhui-rhel-server-rhui-rhscl-7-rpms/7Server/x86_64/primary_db                                                                                                      | 4.7 MB  00:00:00     
        (61/64): rhui-rhel-server-rhui-rhscl-7-source-rpms/7Server/x86_64/group                                                                                                    |  104 B  00:00:00     
        (62/64): rhui-rhel-7-server-rhui-supplementary-source-rpms/7Server/x86_64/primary_db                                                                                       | 4.9 kB  00:00:00     
        (63/64): rhui-rhel-server-rhui-rhscl-7-source-rpms/7Server/x86_64/updateinfo                                                                                               | 439 kB  00:00:00     
        (64/64): rhui-rhel-server-rhui-rhscl-7-source-rpms/7Server/x86_64/primary_db                                                                                               | 1.4 MB  00:00:00     
        repo id                                                                           repo name                                                                                                 status
        rhui-microsoft-azure-rhel7                                                        Microsoft Azure RPMs for Red Hat Enterprise Linux 7                                                            2
        rhui-rhel-7-server-dotnet-rhui-debug-rpms/7Server/x86_64                          dotNET on RHEL Debug RPMs for Red Hat Enterprise Linux 7 Server from RHUI                                     27
        rhui-rhel-7-server-dotnet-rhui-rpms/7Server/x86_64                                dotNET on RHEL RPMs for Red Hat Enterprise Linux 7 Server from RHUI                                           63
        rhui-rhel-7-server-dotnet-rhui-source-rpms/7Server/x86_64                         dotNET on RHEL Source RPMs for Red Hat Enterprise Linux 7 Server from RHUI                                    32
        rhui-rhel-7-server-rhui-debug-rpms/7Server/x86_64                                 Red Hat Enterprise Linux 7 Server from RHUI (Debug RPMs)                                                   6,382
        rhui-rhel-7-server-rhui-extras-debug-rpms/x86_64                                  Red Hat Enterprise Linux 7 Server - Extras from RHUI (Debug RPMs)                                            126
        rhui-rhel-7-server-rhui-extras-rpms/x86_64                                        Red Hat Enterprise Linux 7 Server - Extras from RHUI (RPMs)                                                  709
        rhui-rhel-7-server-rhui-extras-source-rpms/x86_64                                 Red Hat Enterprise Linux 7 Server - Extras from RHUI (Source RPMs)                                           276
        rhui-rhel-7-server-rhui-optional-debug-rpms/7Server/x86_64                        Red Hat Enterprise Linux 7 Server - Optional from RHUI (Debug RPMs)                                        4,263
        rhui-rhel-7-server-rhui-optional-rpms/7Server/x86_64                              Red Hat Enterprise Linux 7 Server - Optional from RHUI (RPMs)                                             13,030
        rhui-rhel-7-server-rhui-optional-source-rpms/7Server/x86_64                       Red Hat Enterprise Linux 7 Server - Optional from RHUI (Source RPMs)                                       3,038
        rhui-rhel-7-server-rhui-rh-common-debug-rpms/7Server/x86_64                       Red Hat Enterprise Linux 7 Server - RH Common from RHUI (Debug RPMs)                                          31
        rhui-rhel-7-server-rhui-rh-common-rpms/7Server/x86_64                             Red Hat Enterprise Linux 7 Server - RH Common from RHUI (RPMs)                                               228
        rhui-rhel-7-server-rhui-rh-common-source-rpms/7Server/x86_64                      Red Hat Enterprise Linux 7 Server - RH Common from RHUI (Source RPMs)                                         89
        rhui-rhel-7-server-rhui-rpms/7Server/x86_64                                       Red Hat Enterprise Linux 7 Server from RHUI (RPMs)                                                        17,720
        rhui-rhel-7-server-rhui-source-rpms/7Server/x86_64                                Red Hat Enterprise Linux 7 Server from RHUI (Source RPMs)                                                  5,185
        rhui-rhel-7-server-rhui-supplementary-debug-rpms/7Server/x86_64                   Red Hat Enterprise Linux 7 Server - Supplementary from RHUI (Debug RPMs)                                       0
        rhui-rhel-7-server-rhui-supplementary-rpms/7Server/x86_64                         Red Hat Enterprise Linux 7 Server - Supplementary from RHUI (RPMs)                                           238
        rhui-rhel-7-server-rhui-supplementary-source-rpms/7Server/x86_64                  Red Hat Enterprise Linux 7 Server - Supplementary from RHUI (Source RPMs)                                      8
        rhui-rhel-server-rhui-rhscl-7-debug-rpms/7Server/x86_64                           Red Hat Software Collections Debug RPMs for Red Hat Enterprise Linux 7 Server from RHUI                      570
        rhui-rhel-server-rhui-rhscl-7-rpms/7Server/x86_64                                 Red Hat Software Collections RPMs for Red Hat Enterprise Linux 7 Server from RHUI                          9,198
        rhui-rhel-server-rhui-rhscl-7-source-rpms/7Server/x86_64                          Red Hat Software Collections Source RPMs for Red Hat Enterprise Linux 7 Server from RHUI                   3,841
        repolist: 65,056
