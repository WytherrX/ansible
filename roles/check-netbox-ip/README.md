Permits to check the next available IP address in a Netbox Prefix
=========

This role permits to find the next available IP address in a Prefix entered by the user in the format 10.10.10.10/24.
It uses prompts to ask the user for the prefix.


Requirements
------------

The community.vmware collection is needed to use this role, you can check whether it is installed by running ``ansible-galaxy collection list``
To install it, use : ``ansible-galaxy collection install netbox.netbox``

Roles Variables
--------------

| Variable         | Required | Type   | Default  | Comments                                                         |
|------------------|----------|--------|----------|------------------------------------------------------------------|
| url_netbox       | yes      | string | None     | URL of the Netbox Server you use (ex : 'https://netbox.test.com')|
| token_netbox     | yes      | string | None     | Your NetBox Token                                                | 
| prefix_f         | yes      | string | None     | Prefix in which you wanna check for the next IP available        |

Example Playbook
----------------

How to use it in your playbooks:

    - hosts: localhost

      roles:
         - check-netbox-ip

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
