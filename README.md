# tf-file "version": 4,
   "terraform_version": "1.5.6",
   "serial": 7,
   "lineage": "553da58b-6921-273f-2884-5fff62ca6d1d",
   "outputs": {
     "ansible_publicIp": {
       "value": "52.8.102.194",
       "type": "string"
     },
     "instance_privateIp": {
       "value": [
         "172.31.17.76",
         "172.31.28.223"
       ],
       "type": [
         "tuple",
         [
           "string",
           "string"
         ]
       ]
     },
     "instance_publicIp": {
       "value": [
         "54.183.139.4",
         "13.56.77.214"
       ],
       "type": [
         "tuple",
         [
           "string",
           "string"
         ]
       ]
     },
     "rhel_privateIp": {
       "value": [
         "172.31.16.28"
       ],
       "type": [
         "tuple",
         [
           "string"
         ]
       ]
     },
     "rhel_publicIp": {
       "value": [
         "54.193.189.239"
       ],
       "type": [
         "tuple",
         [
           "string"
         ]
       ]
     }
   },
   "resources": [
     {
       "mode": "data",
       "type": "aws_ami",
       "name": "rhel",
       "provider": "provider[\"registry.terraform.io/hashicorp/aws\"]",
       "instances": [
         {
           "schema_version": 0,
           "attributes": {
             "architecture": "x86_64",
             "arn": "arn:aws:ec2:us-west-1::image/ami-05816879f7927df75",
             "block_device_mappings": [
               {
                 "device_name": "/dev/sda1",
                 "ebs": {
                   "delete_on_termination": "true",
                   "encrypted": "false",
                   "iops": "0",
                   "snapshot_id": "snap-00c4822b81351a85d",
                   "throughput": "0",
                   "volume_size": "10",
                   "volume_type": "gp2"
                 },
                 "no_device": "",
                 "virtual_name": ""
               }
             ],
             "creation_date": "2023-09-07T03:52:10.000Z",
             "description": "Provided by Red Hat, Inc.",
             "ena_support": true,
             "executable_users": null,
             "filter": [
               {
                 "name": "architecture",
                 "values": [
                   "x86_64"
                 ]
               },
               {
                 "name": "name",
                 "values": [
                   "RHEL-9.2.0_HVM-*-GP2"
                 ]
               },
               {
                 "name": "root-device-type",
                 "values": [
                   "ebs"
                 ]
               },
               {
                 "name": "virtualization-type",
                 "values": [
                   "hvm"
                 ]
               }
             ],
             "hypervisor": "xen",
             "id": "ami-05816879f7927df75",
             "image_id": "ami-05816879f7927df75",
             "image_location": "amazon/RHEL-9.2.0_HVM-20230905-x86_64-38-Hourly2-GP2",
             "image_owner_alias": "amazon",
             "image_type": "machine",
             "kernel_id": null,
             "most_recent": true,
             "name": "RHEL-9.2.0_HVM-20230905-x86_64-38-Hourly2-GP2",
             "name_regex": null,
             "owner_id": "309956199498",
             "owners": [
               "309956199498"
             ],
             "platform": null,
             "platform_details": "Red Hat Enterprise Linux",
             "product_codes": [],
             "public": true,
             "ramdisk_id": null,
             "root_device_name": "/dev/sda1",
             "root_device_type": "ebs",
             "root_snapshot_id": "snap-00c4822b81351a85d",
             "sriov_net_support": "simple",
             "state": "available",
             "state_reason": {
               "code": "UNSET",
               "message": "UNSET"
             },
             "tags": {},
             "usage_operation": "RunInstances:0010",
             "virtualization_type": "hvm"
           },
           "sensitive_attributes": []
         }
       ]
     },
     {
       "mode": "data",
       "type": "aws_ami",
       "name": "ubuntu",
       "provider": "provider[\"registry.terraform.io/hashicorp/aws\"]",
       "instances": [
         {
           "schema_version": 0,
           "attributes": {
             "architecture": "x86_64",
             "arn": "arn:aws:ec2:us-west-1::image/ami-01f808b7a9454bd3b",
             "block_device_mappings": [
               {
                 "device_name": "/dev/sda1",
                 "ebs": {
                   "delete_on_termination": "true",
                   "encrypted": "false",
                   "iops": "0",
                   "snapshot_id": "snap-08f900f206afedc40",
                   "throughput": "0",
                   "volume_size": "8",
                   "volume_type": "gp2"
                 },
                 "no_device": "",
                 "virtual_name": ""
               },
               {
                 "device_name": "/dev/sdb",
                 "ebs": {},
                 "no_device": "",
                 "virtual_name": "ephemeral0"
               },
               {
                 "device_name": "/dev/sdc",
                 "ebs": {},
                 "no_device": "",
                 "virtual_name": "ephemeral1"
               }
             ],
             "creation_date": "2023-09-07T04:28:34.000Z",
             "description": "Canonical, Ubuntu, 22.04 LTS, amd64 jammy image build on 2023-09-07",
             "ena_support": true,
             "executable_users": null,
             "filter": [
               {
                 "name": "architecture",
                 "values": [
                   "x86_64"
                 ]
               },
               {
                 "name": "name",
                 "values": [
                   "ubuntu/images/hvm-ssd/ubuntu-jammy-22.04-amd64-server-*"
                 ]
               },
               {
                 "name": "root-device-type",
                 "values": [
                   "ebs"
                 ]
               },
               {
                 "name": "virtualization-type",
                 "values": [
                   "hvm"
                 ]
               }
             ],
             "hypervisor": "xen",
             "id": "ami-01f808b7a9454bd3b",
             "image_id": "ami-01f808b7a9454bd3b",
             "image_location": "amazon/ubuntu/images/hvm-ssd/ubuntu-jammy-22.04-amd64-server-20230907",
             "image_owner_alias": "amazon",
             "image_type": "machine",
             "kernel_id": null,
             "most_recent": true,
             "name": "ubuntu/images/hvm-ssd/ubuntu-jammy-22.04-amd64-server-20230907",
             "name_regex": null,
             "owner_id": "099720109477",
             "owners": [
               "099720109477"
             ],
             "platform": null,
             "platform_details": "Linux/UNIX",
             "product_codes": [],
             "public": true,
             "ramdisk_id": null,
             "root_device_name": "/dev/sda1",
             "root_device_type": "ebs",
             "root_snapshot_id": "snap-08f900f206afedc40",
             "sriov_net_support": "simple",
             "state": "available",
             "state_reason": {
               "code": "UNSET",
               "message": "UNSET"
             },
             "tags": {},
             "usage_operation": "RunInstances",
             "virtualization_type": "hvm"
           },
           "sensitive_attributes": []
         }
       ]
     },
     {
       "mode": "data",
       "type": "template_cloudinit_config",
       "name": "user-data",
       "provider": "provider[\"registry.terraform.io/hashicorp/template\"]",
       "instances": [
         {
           "schema_version": 0,
           "attributes": {
             "base64_encode": true,
             "gzip": true,
             "id": "2503438349",
             "part": [
               {
                 "content": "#! /bin/bash\nsudo adduser ansible\necho \"ansible:ansible\" | chpasswd\necho \"ansible ALL=(ALL) NOPASSWD:ALL\" | sudo tee /etc/sudoers.d/ansible\nsudo su - ansible\nsudo apt-add-repository ppa:ansible/ansible\nsudo apt install ansible -y\n",
                 "content_type": "text/x-shellscript",
                 "filename": "",
                 "merge_type": ""
               },
               {
                 "content": "#!/bin/bash\n\nsudo apt update\nsudo apt upgrade -y\nsudo apt install software-properties-common apt-transport-https wget -y\nwget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -\nsudo add-apt-repository \"deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main\" -y\nsudo apt install code -y",
                 "content_type": "text/x-shellscript",
                 "filename": "",
                 "merge_type": ""
               }
             ],
             "rendered": "H4sIAAAAAAAA/7xSTW/UMBC9R9r/MIQLHLwGCYEU1EOgPSBlu4jyIYQ4TOzpxtrENp4Ju5H48cih2922SNw4WfP8/N7TG78NXsiL+jhFqmAYe3ERk+jB7cm+hjaM3mKazsrVu9XFm/Wny/P6w9eyyJP6TIld8BU8Xz5bFItCqVPSorjVTuj5mpK68CZY5zcVvGqdnBBmc6G96L3ijvqeTXJRFsXKDfTA5/Ej0K3zukXuCh5tALR2ZEqAnl3bU0GmC1DeTNXNWcIvMF1E5p29y4C6ac6e1E3zFC7X7+urqy/nVd00+cEsL0SgSYzOEyVeWn1wmu95BAV3EIyi0FqVKAZ2EtIEMeIhib7PBedZsO8PIqCm/9rnsc5jpDFaFDqdNwntHO1BbA7XssNEKqYQKYkjViYMQ/BzE5IDx5BEdSKRYbchyTp/zh8wo5XWEc0WN8TLwZkUsujShEFvaWJ9hJANqLU6LCcbbGnKfwDU7XdQGT5pv7TUwjdMpjvDwb588f1fpvNb/ZNNsAQsmLcyoPPlXwuYWWq6vzOlFsXvAAAA///tjdwuYgMAAA=="
           },
           "sensitive_attributes": []
         }
       ]
     },
     {
       "mode": "managed",
       "type": "aws_instance",
       "name": "rhel-hosts",
       "provider": "provider[\"registry.terraform.io/hashicorp/aws\"]",
       "instances": [
         {
           "index_key": 0,
           "schema_version": 1,
           "attributes": {
             "ami": "ami-05816879f7927df75",
             "arn": "arn:aws:ec2:us-west-1:411854276167:instance/i-0e1fd01a6b8705b96",
             "associate_public_ip_address": true,
             "availability_zone": "us-west-1a",
             "capacity_reservation_specification": [
               {
                 "capacity_reservation_preference": "open",
                 "capacity_reservation_target": []
               }
             ],
             "cpu_core_count": 1,
             "cpu_threads_per_core": 1,
             "credit_specification": [
               {
                 "cpu_credits": "standard"
               }
             ],
             "disable_api_termination": false,
             "ebs_block_device": [],
             "ebs_optimized": false,
             "enclave_options": [
               {
                 "enabled": false
               }
             ],
             "ephemeral_block_device": [],
             "get_password_data": false,
             "hibernation": false,
             "host_id": null,
             "iam_instance_profile": "",
             "id": "i-0e1fd01a6b8705b96",
             "instance_initiated_shutdown_behavior": "stop",
             "instance_state": "running",
             "instance_type": "t2.micro",
             "ipv6_address_count": 0,
             "ipv6_addresses": [],
             "key_name": "ansible-key",
             "launch_template": [],
             "metadata_options": [
               {
                 "http_endpoint": "enabled",
                 "http_put_response_hop_limit": 1,
                 "http_tokens": "optional",
                 "instance_metadata_tags": "disabled"
               }
             ],
             "monitoring": false,
             "network_interface": [],
             "outpost_arn": "",
             "password_data": "",
             "placement_group": "",
             "placement_partition_number": null,
             "primary_network_interface_id": "eni-00238885d684fe088",
             "private_dns": "ip-172-31-16-28.us-west-1.compute.internal",
             "private_ip": "172.31.16.28",
             "public_dns": "ec2-54-193-189-239.us-west-1.compute.amazonaws.com",
             "public_ip": "54.193.189.239",
             "root_block_device": [
               {
                 "delete_on_termination": true,
                 "device_name": "/dev/sda1",
                 "encrypted": false,
                 "iops": 100,
                 "kms_key_id": "",
                 "tags": {},
                 "throughput": 0,
                 "volume_id": "vol-00e59637eae6e4dda",
                 "volume_size": 10,
                 "volume_type": "gp2"
               }
             ],
             "secondary_private_ips": [],
             "security_groups": [
               "default"
             ],
             "source_dest_check": true,
             "subnet_id": "subnet-4cc7422a",
             "tags": {
               "Name": "My-rhel-0"
             },
             "tags_all": {
               "Name": "My-rhel-0"
             },
             "tenancy": "default",
             "timeouts": null,
             "user_data": "30c811f45ae0d70578859538fe08e769d907f842",
             "user_data_base64": null,
             "volume_tags": null,
             "vpc_security_group_ids": [
               "sg-7d59470b"
             ]
           },
           "sensitive_attributes": [],
           "private": "eyJlMmJmYjczMC1lY2FhLTExZTYtOGY4OC0zNDM2M2JjN2M0YzAiOnsiY3JlYXRlIjo2MDAwMDAwMDAwMDAsImRlbGV0ZSI6MTIwMDAwMDAwMDAwMCwidXBkYXRlIjo2MDAwMDAwMDAwMDB9LCJzY2hlbWFfdmVyc2lvbiI6IjEifQ==",
           "dependencies": [
             "data.aws_ami.rhel"
           ]
         }
       ]
     },
     {
       "mode": "managed",
       "type": "aws_instance",
       "name": "ubuntu",
       "provider": "provider[\"registry.terraform.io/hashicorp/aws\"]",
       "instances": [
         {
           "schema_version": 1,
           "attributes": {
             "ami": "ami-01f808b7a9454bd3b",
             "arn": "arn:aws:ec2:us-west-1:411854276167:instance/i-01543deed37b584ae",
             "associate_public_ip_address": true,
             "availability_zone": "us-west-1a",
             "capacity_reservation_specification": [
               {
                 "capacity_reservation_preference": "open",
                 "capacity_reservation_target": []
               }
             ],
             "cpu_core_count": 1,
             "cpu_threads_per_core": 1,
             "credit_specification": [
               {
                 "cpu_credits": "standard"
               }
             ],
             "disable_api_termination": false,
             "ebs_block_device": [],
             "ebs_optimized": false,
             "enclave_options": [
               {
                 "enabled": false
               }
             ],
             "ephemeral_block_device": [],
             "get_password_data": false,
             "hibernation": false,
             "host_id": null,
             "iam_instance_profile": "",
             "id": "i-01543deed37b584ae",
             "instance_initiated_shutdown_behavior": "stop",
             "instance_state": "running",
             "instance_type": "t2.micro",
             "ipv6_address_count": 0,
             "ipv6_addresses": [],
             "key_name": "ansible-key",
             "launch_template": [],
             "metadata_options": [
               {
                 "http_endpoint": "enabled",
                 "http_put_response_hop_limit": 1,
                 "http_tokens": "optional",
                 "instance_metadata_tags": "disabled"
               }
             ],
             "monitoring": false,
             "network_interface": [],
             "outpost_arn": "",
             "password_data": "",
             "placement_group": "",
             "placement_partition_number": null,
             "primary_network_interface_id": "eni-0271a52a464ce7f7a",
             "private_dns": "ip-172-31-17-135.us-west-1.compute.internal",
             "private_ip": "172.31.17.135",
             "public_dns": "ec2-52-8-102-194.us-west-1.compute.amazonaws.com",
             "public_ip": "52.8.102.194",
             "root_block_device": [
               {
                 "delete_on_termination": true,
                 "device_name": "/dev/sda1",
                 "encrypted": false,
                 "iops": 100,
                 "kms_key_id": "",
                 "tags": {},
                 "throughput": 0,
                 "volume_id": "vol-0a448815cac8b9094",
                 "volume_size": 8,
                 "volume_type": "gp2"
               }
             ],
             "secondary_private_ips": [],
             "security_groups": [
               "default"
             ],
             "source_dest_check": true,
             "subnet_id": "subnet-4cc7422a",
             "tags": {
               "Name": "Ansible-Ubuntu"
             },
             "tags_all": {
               "Name": "Ansible-Ubuntu"
             },
             "tenancy": "default",
             "timeouts": null,
             "user_data": "f6c044da833ba47247e348f0cc6ce891c1c62e3b",
             "user_data_base64": null,
             "volume_tags": null,
             "vpc_security_group_ids": [
               "sg-7d59470b"
             ]
           },
           "sensitive_attributes": [],
           "private": "eyJlMmJmYjczMC1lY2FhLTExZTYtOGY4OC0zNDM2M2JjN2M0YzAiOnsiY3JlYXRlIjo2MDAwMDAwMDAwMDAsImRlbGV0ZSI6MTIwMDAwMDAwMDAwMCwidXBkYXRlIjo2MDAwMDAwMDAwMDB9LCJzY2hlbWFfdmVyc2lvbiI6IjEifQ==",
           "dependencies": [
             "data.aws_ami.ubuntu",
             "data.template_cloudinit_config.user-data"
           ]
         }
       ]
     },
     {
       "mode": "managed",
       "type": "aws_instance",
       "name": "ubuntu-hosts",
       "provider": "provider[\"registry.terraform.io/hashicorp/aws\"]",
       "instances": [
         {
           "index_key": 0,
           "schema_version": 1,
           "attributes": {
             "ami": "ami-01f808b7a9454bd3b",
             "arn": "arn:aws:ec2:us-west-1:411854276167:instance/i-078fbca696d9f1901",
             "associate_public_ip_address": true,
             "availability_zone": "us-west-1a",
             "capacity_reservation_specification": [
               {
                 "capacity_reservation_preference": "open",
                 "capacity_reservation_target": []
               }
             ],
             "cpu_core_count": 1,
             "cpu_threads_per_core": 1,
             "credit_specification": [
               {
                 "cpu_credits": "standard"
               }
             ],
             "disable_api_termination": false,
             "ebs_block_device": [],
             "ebs_optimized": false,
             "enclave_options": [
               {
                 "enabled": false
               }
             ],
             "ephemeral_block_device": [],
             "get_password_data": false,
             "hibernation": false,
             "host_id": null,
             "iam_instance_profile": "",
             "id": "i-078fbca696d9f1901",
             "instance_initiated_shutdown_behavior": "stop",
             "instance_state": "running",
             "instance_type": "t2.micro",
             "ipv6_address_count": 0,
             "ipv6_addresses": [],
             "key_name": "ansible-key",
             "launch_template": [],
             "metadata_options": [
               {
                 "http_endpoint": "enabled",
                 "http_put_response_hop_limit": 1,
                 "http_tokens": "optional",
                 "instance_metadata_tags": "disabled"
               }
             ],
             "monitoring": false,
             "network_interface": [],
             "outpost_arn": "",
             "password_data": "",
             "placement_group": "",
             "placement_partition_number": null,
             "primary_network_interface_id": "eni-0e47e4077e1ebd503",
             "private_dns": "ip-172-31-17-76.us-west-1.compute.internal",
             "private_ip": "172.31.17.76",
             "public_dns": "ec2-54-183-139-4.us-west-1.compute.amazonaws.com",
             "public_ip": "54.183.139.4",
             "root_block_device": [
               {
                 "delete_on_termination": true,
                 "device_name": "/dev/sda1",
                 "encrypted": false,
                 "iops": 100,
                 "kms_key_id": "",
                 "tags": {},
                 "throughput": 0,
                 "volume_id": "vol-061986cc30556351e",
                 "volume_size": 8,
                 "volume_type": "gp2"
               }
             ],
             "secondary_private_ips": [],
             "security_groups": [
               "default"
             ],
             "source_dest_check": true,
             "subnet_id": "subnet-4cc7422a",
             "tags": {
               "Name": "My-Ubuntu-0",
               "Type": "My-Ubuntu-0"
             },
             "tags_all": {
               "Name": "My-Ubuntu-0",
               "Type": "My-Ubuntu-0"
             },
             "tenancy": "default",
             "timeouts": null,
             "user_data": "30c811f45ae0d70578859538fe08e769d907f842",
             "user_data_base64": null,
             "volume_tags": null,
             "vpc_security_group_ids": [
               "sg-7d59470b"
             ]
           },
           "sensitive_attributes": [],
           "private": "eyJlMmJmYjczMC1lY2FhLTExZTYtOGY4OC0zNDM2M2JjN2M0YzAiOnsiY3JlYXRlIjo2MDAwMDAwMDAwMDAsImRlbGV0ZSI6MTIwMDAwMDAwMDAwMCwidXBkYXRlIjo2MDAwMDAwMDAwMDB9LCJzY2hlbWFfdmVyc2lvbiI6IjEifQ==",
           "dependencies": [
             "data.aws_ami.ubuntu"
           ]
         },
         {
           "index_key": 1,
           "schema_version": 1,
           "attributes": {
             "ami": "ami-01f808b7a9454bd3b",
             "arn": "arn:aws:ec2:us-west-1:411854276167:instance/i-0b42af1e854bd3872",
             "associate_public_ip_address": true,
             "availability_zone": "us-west-1a",
             "capacity_reservation_specification": [
               {
                 "capacity_reservation_preference": "open",
                 "capacity_reservation_target": []
               }
             ],
             "cpu_core_count": 1,
             "cpu_threads_per_core": 1,
             "credit_specification": [
               {
                 "cpu_credits": "standard"
               }
             ],
             "disable_api_termination": false,
             "ebs_block_device": [],
             "ebs_optimized": false,
             "enclave_options": [
               {
                 "enabled": false
               }
             ],
             "ephemeral_block_device": [],
             "get_password_data": false,
             "hibernation": false,
             "host_id": null,
             "iam_instance_profile": "",
             "id": "i-0b42af1e854bd3872",
             "instance_initiated_shutdown_behavior": "stop",
             "instance_state": "running",
             "instance_type": "t2.micro",
             "ipv6_address_count": 0,
             "ipv6_addresses": [],
             "key_name": "ansible-key",
             "launch_template": [],
             "metadata_options": [
               {
                 "http_endpoint": "enabled",
                 "http_put_response_hop_limit": 1,
                 "http_tokens": "optional",
                 "instance_metadata_tags": "disabled"
               }
             ],
             "monitoring": false,
             "network_interface": [],
             "outpost_arn": "",
             "password_data": "",
             "placement_group": "",
             "placement_partition_number": null,
             "primary_network_interface_id": "eni-0efd456a98d6e0437",
             "private_dns": "ip-172-31-28-223.us-west-1.compute.internal",
             "private_ip": "172.31.28.223",
             "public_dns": "ec2-13-56-77-214.us-west-1.compute.amazonaws.com",
             "public_ip": "13.56.77.214",
             "root_block_device": [
               {
                 "delete_on_termination": true,
                 "device_name": "/dev/sda1",
                 "encrypted": false,
                 "iops": 100,
                 "kms_key_id": "",
                 "tags": {},
                 "throughput": 0,
                 "volume_id": "vol-008ac821560267bb1",
                 "volume_size": 8,
                 "volume_type": "gp2"
               }
             ],
             "secondary_private_ips": [],
             "security_groups": [
               "default"
             ],
             "source_dest_check": true,
             "subnet_id": "subnet-4cc7422a",
             "tags": {
               "Name": "My-Ubuntu-1",
               "Type": "My-Ubuntu-1"
             },
             "tags_all": {
               "Name": "My-Ubuntu-1",
               "Type": "My-Ubuntu-1"
             },
             "tenancy": "default",
             "timeouts": null,
             "user_data": "30c811f45ae0d70578859538fe08e769d907f842",
             "user_data_base64": null,
             "volume_tags": null,
             "vpc_security_group_ids": [
               "sg-7d59470b"
             ]
           },
           "sensitive_attributes": [],
           "private": "eyJlMmJmYjczMC1lY2FhLTExZTYtOGY4OC0zNDM2M2JjN2M0YzAiOnsiY3JlYXRlIjo2MDAwMDAwMDAwMDAsImRlbGV0ZSI6MTIwMDAwMDAwMDAwMCwidXBkYXRlIjo2MDAwMDAwMDAwMDB9LCJzY2hlbWFfdmVyc2lvbiI6IjEifQ==",
           "dependencies": [
             "data.aws_ami.ubuntu"
           ]
         }
       ]
     },
     {
       "mode": "managed",
       "type": "null_resource",
       "name": "vscode-config",
       "provider": "provider[\"registry.terraform.io/hashicorp/null\"]",
       "instances": [
         {
           "schema_version": 0,
           "attributes": {
             "id": "5716385555669993552",
             "triggers": null
           },
           "sensitive_attributes": [],
           "dependencies": [
             "aws_instance.ubuntu",
             "data.aws_ami.ubuntu",
             "data.template_cloudinit_config.user-data",
             "time_sleep.wait_for_instance"
           ]
         }
       ]
     },
     {
       "mode": "managed",
       "type": "time_sleep",
       "name": "wait_for_instance",
       "provider": "provider[\"registry.terraform.io/hashicorp/time\"]",
       "instances": [
         {
           "schema_version": 0,
           "attributes": {
             "create_duration": "180s",
             "destroy_duration": null,
             "id": "2023-09-15T02:46:37Z",
             "triggers": null
           },
           "sensitive_attributes": [],
           "dependencies": [
             "aws_instance.ubuntu",
             "data.aws_ami.ubuntu",
             "data.template_cloudinit_config.user-data"
           ]
         }
       ]
     }
   ],
   "check_results": null
 }
