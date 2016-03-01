oracle-weblogic
===============

Ansible role to execute the oracle weblogic scripting tool

Requirements
------------

Oracle Weblogic

Variables 
---------

-  oracle_wlst_execute: yes
-  oracle_wlst_oracle_home: /opt/oraclefmw/product/oracle_home
-  oracle_wlst_create_domain: yes
-  oracle_wlst_create_domain_domains_home: /home/oraclefmw/config/domains #
-  oracle_wlst_create_domain_applications_home: /home/oraclefmw/config/apps #
-  oracle_wlst_create_domain_info:
-    name: local #
-    templates:
-      -
-        name: Basic WebLogic Server Domain
-        version: 10.3.6
-    adminserver:
-      name: AdminServer
-      listen_address:
-      listen_port: 7101
-    adminuser:
-      username: weblogic
-      password: welcome1
-    custom_datasources:
-      -
-        name: 
-        targets: AdminServer
-        jdbc_driver: oracle.jdbc.OracleDriver
-        jdbc_url: jdbc:oracle:thin:@local-osi-db:1521:FMWDB
-        schema_username: USER
-        schema_password: welcome1
-    filestores:
-        -
-          name: 
-          directory: 
-          targets: 
-    messaging:
-      jms_servers:
-        -
-          name: 
-          filestore: 
-          targets: 
-          jms_modules:
-            -
-              name: 
-              subdeployment: 
-              targets: 
-              connection_factories:
-                -
-                  name: 
-              queues:
-                -
-                  name: 


Credits
-----------

- Jorge Quilcate (https://github.com/jeqo) for making the templates
- Diego Otoya (https://github.com/TheDotHub) for fixing some vars
