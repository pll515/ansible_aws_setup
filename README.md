
# ansible_bagel


Ansible repository for AWS Simple VPC Deployment


---Pre-requisite---

You only need an AWS Account and access to an Admin User.

---Instructions---

1. Create a vault file with AWS credentials

    1.1 Run:  `ansible-vault create aws_keys.yml`
        
    1.2 Update file as following:
    
       aws_access_key: AKIAJLHNMCBOITV643U
       aws_secret_key: iMcMw4TB7cv9k+bdLqMGHKSTQIsZD43RVuSKFnUt

2.  Run: `ansible-playbook aws_vpc.yml`

Done :) 


TODO

- [ ] Add a Schema of the VPC 

---Deprecated---

To launch instances on AWS run : ansible-playbook -i host.ini --ask-vault aws_ec2.yml
-> Make sure you have the good key pairs (aws_ec2) and good path to it (group_vars)


When done kill all instances tagged "temporary" with : ansible-playbook --ask-vault aws_kill_temp_ec2.yml



