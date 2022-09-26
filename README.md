# Ansible-AWS
Ansible project for creating AWS EC2 instances

Requirements \
The below requirements are needed on the host that executes this module:\
`boto`\
`boto3` >= 1.16.0\
`botocore` >= 1.19.0\
`python` >= 3.6


Ansible mdule `Install anazon.aws.ec2` with following command:
```
ansible-galaxy collection install amazon.aws
```

# VM Provisioning

### Step 1: Modify vars.yml
Put your AWS credentials
 * `access_key`
 * `secret_key`

Modify other variables depending on `region` and `instance_type`

### Step 2: Check Ansible playbook
```bash
ansible-playbook run.yml --check -vvv
```

### Step 3: Start Ansible playbook
```bash
ansible-playbook run.yml -v
```




