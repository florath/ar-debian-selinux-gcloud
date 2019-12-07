Ansible Role for enabling SELinux on Debian on Google Cloud
***********************************************************
When running Debian on Google Cloud only using the default SELinux
policy boot will fail.  This Ansible Role installes SELinux with the
needed rules that it works on Google Cloud.

Usage
-----

Put this into the requirements.yaml file:

.. code:: bash

   - src: https://github.com/florath/ar-debian-selinux-gcloud
     name: debian-selinux-gcloud

and add this as a role:
     
.. code:: bash

   roles:
    - debian-selinux-gcloud
