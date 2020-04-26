# NodeApp Packer linking to Terraform

## Prerequisites:
- Chef
- AWS CLI
- Git
- Your own .pem key

## How to clone this repo:
In your terminal, please type in the following:
```
git clone git@github.com:atahar123/packer-terraform.git
```

### Lines to change
- Change the following to your own .pem key, its path.
- Change the AMI name to your name.
```
13     "ssh_keypair_name": "atahar-eng54",
14     "ssh_private_key_file": "~/.ssh/atahar-eng54.pem",
31     "ami_name": "atahar-terraform"
```

# How to install
Run the following to link the ```node``` cookbook locally. You must do this:
```
berks vendor
```

Next, validate the packer:
```
packer validate packer_nodejs.json
```
This should show a successful message.


Next, build the AMI:
```
packer build packer_nodejs.json
```


Once that's done, you should go to AMIs in AWS and put in the name you had in line 31.
