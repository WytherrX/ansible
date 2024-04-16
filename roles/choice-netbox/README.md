Permits to find a prefix from an existing site in Netbox using prompts
=========

This role permits to find a prefix linked to a VLAN used in a Site.
It uses prompts to ask the user for a Site and then display the VLANS used in this Site.
Then, it asks the user which VLAN he is interested in and which prefix to use in this VLAN.

/!\ It is used here in order to create a Virtual Machine in Netbox, so if you want to adjust it for your usage, change the different prints in the prompts. 


Requirements
------------

The community.vmware collection is needed to use this role, you can check whether it is installed by running ``ansible-galaxy collection list``
To install it, use : ``ansible-galaxy collection install netbox.netbox``
It also require ``pynetbox`` which can be installed on Ubuntu (for example) by using ``apt install python3-pynetbox``

Role Variables
--------------

| Variable         | Required | Type   | Default  | Comments                                                          |
|------------------|----------|--------|----------|-------------------------------------------------------------------|
| url_netbox       | yes      | string | None     | URL of the Netbox Server you use (ex : 'https://netbox.test.com') |            
| token_netbox     | yes      | string | None     | Your NetBox Token                                                 | 


Example Playbook
----------------

How to use it in your playbooks:

    - hosts: localhost

      roles:
         - choice-netbox

License
-------

This is free and unencumbered software released into the public domain.

Anyone is free to copy, modify, publish, use, compile, sell, or
distribute this software, either in source code form or as a compiled
binary, for any purpose, commercial or non-commercial, and by any
means.

In jurisdictions that recognize copyright laws, the author or authors
of this software dedicate any and all copyright interest in the
software to the public domain. We make this dedication for the benefit
of the public at large and to the detriment of our heirs and
successors. We intend this dedication to be an overt act of
relinquishment in perpetuity of all present and future rights to this
software under copyright law.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.

For more information, please refer to <https://unlicense.org>


Author Information
------------------

Wytherr 
