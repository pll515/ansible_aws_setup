
# ansible_bagel


Ansible repository for AWS Simple VPC Deployment

i
---Pre-requisite---

You only need an AWS Account and access to an Admin User.
i
---Instructions---

1. Create a vault file with AWS credentials

    1.1 Go to root and execute this command:  `ansible-vault create aws_keys.yml`
        
    1.2 Update the newly created file with the following informations (you can only update once with a vault file):
    You can find your aws credentials in the security credentials tab on AWS console.

       aws_access_key: AKIAJLHNMCBOITV643U
       aws_secret_key: iMcMw4TB7cv9k+bdLqMGHKSTQIsZD43RVuSKFnUt

2.  Run: `ansible-playbook aws_vpc.yml`

Done :) 


TODO

- [ ] Add a Schema of the VPC 



