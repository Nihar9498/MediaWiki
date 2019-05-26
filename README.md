# Cloudformation template to create EC2s , RDS, ELB
aws cloudformation create-stack --stack-name ec2-db-elb --template-body file://cloudformation/ec2-db-elb.json --parameters DBPwd="dbpassword"
# Wiki Playbook
This Ansible playbook deploys an instance of MediaWiki on EC2.
ansible-playbook -i aws site.yml --extra-vars "$@"
