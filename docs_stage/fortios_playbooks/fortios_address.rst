===============
fortios_address
===============


Playbook Task Examples
----------------------

.. code-block:: yaml

    - name: Register french addresses
      fortios_address:
        host: 192.168.0.254
        username: admin
        password: p4ssw0rd
        state: present
        name: "fromfrance"
        type: geography
        country: FR
        comment: "French geoip address"
    
    - name: Register some fqdn
      fortios_address:
        host: 192.168.0.254
        username: admin
        password: p4ssw0rd
        state: present
        name: "Ansible"
        type: fqdn
        value: www.ansible.com
        comment: "Ansible website"
    
    - name: Register google DNS
      fortios_address:
        host: 192.168.0.254
        username: admin
        password: p4ssw0rd
        state: present
        name: "google_dns"
        type: ipmask
        value: 8.8.8.8
    



Playbook File Examples
----------------------

%%PB_FILE_EXAMPLE_TOKEN%%

