create ping/pong Nginx service using ansible

before using you must have ssh key pair and configure security group in you aws region

1 step open vars.yml and set variables:

    hostname: not set
    ec2_access_key: "you access key"
    ec2_secret_key: "you ssecret key"
    group: "set security group"
    region: "set region"
    ec2_availability_zone: "not set"
    ec2_availability_zone2: "not set"
    keypair: "set keypair name"
    ami_name: "not set"
    vpc_id: "vpc-set"
    subnet_id: "subnet-set"

2 step run coomand:

	ansible-playbook playbook.yml --private-key=/path/you/private/key.pem