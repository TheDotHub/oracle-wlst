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


Credits
-----------

- Jorge Quilcate (https://github.com/jeqo) for making the templates
- Diego Otoya (https://github.com/TheDotHub) for fixing some vars
