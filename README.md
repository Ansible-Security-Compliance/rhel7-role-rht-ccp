Red Hat Corporate Profile for Certified Cloud Providers (RH CCP)
=========

Ansible remediation role for profile rht-ccp  
Profile Title:  Red Hat Corporate Profile for Certified Cloud Providers (RH CCP)  
Profile Description:  
This is a *draft* SCAP profile for Red Hat Certified Cloud Providers.  
  
Benchmark ID:  RHEL-7  
Benchmark Version:  0.1.38  
  
XCCDF Version:  1.1  
  
This file was generated by OpenSCAP 1.2.17 using:  
	$ oscap xccdf generate fix --profile rht-ccp --template urn:xccdf:fix:script:ansible xccdf-file.xml   
  
This script is generated from an OpenSCAP profile without preliminary evaluation.  
It attempts to fix every selected rule, even if the system is already compliant.  
  
How to apply this remediation role:  
$ ansible-playbook -i "192.168.1.155," playbook.yml  
$ ansible-playbook -i inventory.ini playbook.yml

Requirements
------------

N/A

Role Variables
--------------

To customize the role to your liking, check out the [list of variables](vars/main.yml).

Dependencies
------------

N/A

Example Playbook
----------------

Run `ansible-galaxy install Ansible-Security-Compliance.rhel7-role-rht-ccp` to
download and install the role. Then you can use the following playbook snippet.


    - hosts: all
      roles:
         - { role: Ansible-Security-Compliance.rhel7-role-rht-ccp }


Then first check the playbook using (on the localhost):

    ansible-playbook -i "localhost," -c local --check playbook.yml

To deploy it, use (this may change configuration of your local machine!):

    ansible-playbook -i "localhost," -c local playbook.yml


License
-------

BSD-3-Clause

Author Information
------------------

This Ansible remediation role has been generated from the body of security policies developed by the SCAP Security Guide project. Please see https://github.com/OpenSCAP/scap-security-guide/blob/master/Contributors.md for an updated list of authors and contributors.
