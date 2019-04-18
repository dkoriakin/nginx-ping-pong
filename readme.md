create ping/pong Nginx service using ancible

before using you must have ssh key pair and configure security group in you aws region

1 step open playbook.yml and set variables:

    ec2_access_key: "you access key"
    ec2_secret_key: "you ssecret key"
    group: "set security group"
    region: "set region"
    keypair: "set keypair name"

2 step run coomand:

	ancible-playbook playbook.yml --private-key=/path/you/private/key.pem