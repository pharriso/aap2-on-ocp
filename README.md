Deloy AAP2 on OCP
=========

Some example OCP yaml files in the ocp-files directory and a playbook to deploy a basic example of AAP on OCP.

Running the playbook.
------------

Run the playbook from the CLI with ansible-navigator. The ee-supported image contains all of the pre-reqs.

```
ansible-navigator run deploy_controller.yml -m stdout -u root --private-key ~/.ssh/demolab_id_rsa -i ignite.demolab.local, -e ocp_name=clarksdale -e replicas=1 -e ocp_namespace=pharriso -e ocp_password=Redhat123```
