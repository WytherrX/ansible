Cloning a template/VM in the emptiest datastore in vSphere
=========

This role permits to clone a Virtual Machine in vSphere from an already existing template or Virtual Machine.
It is also set up to use the emptiest datastore as the storage for the new Virtual Machine.

Requirements
------------

The community.vmware collection is needed to use this role, you can check whether it is installed by running ``ansible-galaxy collection list``
To install it, use : ``ansible-galaxy collection install community.vmware``

Role Variables
--------------

| Variable         | Required | Type   | Default  | Comments                                           |
|------------------|----------|--------|----------|----------------------------------------------------|
| vcenter_hostname | yes      | string | None     | Hostname or IP Address of the vSphere vCenter      |
| vcenter_username | yes      | string | None     | The username of the vSphere user the role will use |
| vcenter_password | yes      | string | None     | The password of the vSphere user the role will use |
| datacenter       | yes      | string | None     | Datacenter where the template/VM is stored         |
| folder           | yes      | string | /        | Destination folder, use the absolute path          |
| clone_vm         | yes      | string | NewVM    | Name of the new VM the role will create            |
| template_vm      | yes      | string | None     | Name of the template/VM you want to clone          | 

Example Playbook
----------------

How to use it in your playbooks:

    - hosts: localhost

      roles:
         - template-to-vm

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
