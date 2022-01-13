# cspUtility

This utility image is built for using ansible and targeting specific cloud serivc

### Installed Packages (rpm, pip)
| Packages |
| ------- |
| ansible |
| openshift |
| boto3 |
| botocore |
| awscli | 
| azure-cli |
| pyOpenSSL |
| passlib |
| requests |
| cryptography |
| terraform |
| git |
| python3 |
| openssh-clients |

### Ansible Collections
| Ansible Collections |
| ------------------- |
| kubernetes.core |
| containers.podman |


### Version outputs
```bash
terraform -v
Terraform v1.1.3
```

```bash
ansible-playbook [core 2.11.7]
  config file = None
  configured module search path = ['/root/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
  ansible python module location = /usr/local/lib/python3.6/site-packages/ansible
  ansible collection location = /root/.ansible/collections:/usr/share/ansible/collections
  executable location = /usr/local/bin/ansible-playbook
  python version = 3.6.8 (default, Sep  9 2021, 07:49:02) [GCC 8.5.0 20210514 (Red Hat 8.5.0-3)]
  jinja version = 3.0.3
  libyaml = True
```
### Entrypoint information
The default entrypoint for the image is `/bin/bash/`

### Usage
`podman run quay.io/jrickard0/cspUtility:v1 ansible-playbook <playbook_name>.yml -e <extra_var> `