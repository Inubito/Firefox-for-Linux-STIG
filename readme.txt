I noticed that a majority of the Firefox STIG scripts have been created as an Ansible playbook. This file is intended for those who do not have Ansible or require a standalone file to configure Firefox according to STIG (accurate as of V6R5).

Also, other Firefox hardening guides are still using the old mozilla.cfg file while the newer requirements call for a policies.json.

This JSON file contains required STIG changes for all checks from Evaluate-STIG. 3 manual checks must still be conducted.

For RedHat users, this will need to be placed in the /usr/lib64/firefox/distributions folder and given read permissions for Firefox to access the policies. Your distribution may vary.
