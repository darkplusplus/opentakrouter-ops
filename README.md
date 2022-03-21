# opentakrouter

this role implements management of opentakrouter. this is currently not a comprehensive deployment, but rather a quickstart or a framework to get you started.

## quickstart

This assumes using deploying a new server on ec2 and you already have ansible installed.


1. Provision a new ec2 instance. Have your keypair and know how to access your host. Examine the configuration template to understand the potential security group configuration to allow traffic.
2. Update the `hosts` inventory file with your ec2 instance name.
3. Run the playbook. This might look like:
```
$ ansible-playbook -i hosts site.yml --private-key ~/.ssh/foo.pem
```
4. Browse to the admin page on port 8080.
