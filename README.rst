========================
Team and repository tags
========================

.. image:: https://governance.openstack.org/tc/badges/openstack-ansible-os_zaqar.svg
    :target: https://governance.openstack.org/tc/reference/tags/index.html

.. Change things from this point on

OpenStack-Ansible Zaqar
#######################
:tags: openstack, zaqar, cloud, ansible
:category: \*nix

This Ansible role installs and configures OpenStack Zaqar.

Linux Distribution Support:  Ubuntu 14.04

Default Variables
=================

.. literalinclude:: ../../defaults/main.yml
   :language: yaml
   :start-after: under the License.

Required Variables
==================

(to be completed)

Example Playbook
================

.. code-block:: yaml

   - name: Install zaqar service
     hosts: zaqar_all
     user: root
     roles:
       - role: "os_zaqar"
         zaqar_local_mode: true
         zaqar_install_nginx: true
         zaqar_api_bind_address: 192.168.33.11
         zaqar_mgmt_db_connection_string: 'sqlite:////tmp/zaqar.db'

================================
Zaqar role for OpenStack-Ansible
================================

Ansible role to install OpenStack Zaqar.

Documentation for the project can be found at:
  https://docs.openstack.org/openstack-ansible-os_zaqar/latest/

Release notes for the project can be found at:
  https://docs.openstack.org/releasenotes/openstack-ansible-os_zaqar/

The project home is at:
  https://launchpad.net/openstack-ansible
