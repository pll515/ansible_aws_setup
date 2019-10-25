
# ansible_bagel


Ansible repository for AWS Simple VPC Deployment


---Pre-requisite---

You only need an AWS Account and an Admin User credentials.

---Instructions---

1. Create a vault file with AWS credentials

    1.1 Go to root of this project and execute this command:  `ansible-vault create aws_keys.yml`
    
    1.2 Choose a password 
    
    1.3 Update the newly created file with the following information:

       aws_access_key: AKIAJLHNMCBOITV643U
       aws_secret_key: iMcMw4TB7cv9k+bdLqMGHKSTQIsZD43RVuSKFnUt 
       
     *You can find your aws credentials in the security credentials tab on AWS console.
     
     *You can only update this file at creation, if you make an error, try again

2.  Run: `ansible-playbook aws_vpc.yml`

Done :) 




