OpenStack-Ansible Zaqar
#######################
:tags: openstack, zaqar, cloud, ansible
:category: \*nix

This Ansible role installs and configures OpenStack Zaqar.

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

   - name: Install zaqar server
     hosts: zaqar_all
     user: root
     roles:
       - role: "os_zaqar"
         zaqar_local_mode: true
         zaqar_install_nginx: true
         zaqar_api_bind_address: 192.168.33.11
         zaqar_mgmt_db_connection_string: 'sqlite:////tmp/zaqar.db'
