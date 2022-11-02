+++
title = "Terraform Docs"
description = "This is an area for technical documentation"
weight = 4
+++
<!-- BEGIN_TF_DOCS -->


## Required Inputs

No required inputs.

## Optional Inputs

The following input variables are optional (have default values):

### <a name="input_aws_access_key"></a> [aws\_access\_key](#input\_aws\_access\_key)

Description: Precreated AWS access key.

Type: `string`

Default: `""`

### <a name="input_aws_ecr_region"></a> [aws\_ecr\_region](#input\_aws\_ecr\_region)

Description: AWS ECR region.

Type: `string`

Default: `"us-west-2"`

### <a name="input_aws_region"></a> [aws\_region](#input\_aws\_region)

Description: AWS region.

Type: `string`

Default: `"us-west-2"`

### <a name="input_aws_s3_backup_bucket"></a> [aws\_s3\_backup\_bucket](#input\_aws\_s3\_backup\_bucket)

Description: s3 backup backet name

Type: `string`

Default: `"se-tpm-develop-backup-bucket"`

### <a name="input_aws_secret_key"></a> [aws\_secret\_key](#input\_aws\_secret\_key)

Description: Precreated AWS secret key.

Type: `string`

Default: `""`

### <a name="input_backend_port"></a> [backend\_port](#input\_backend\_port)

Description: The port the service on the EKS instances listen on.

Type: `number`

Default: `31306`

### <a name="input_backend_protocol"></a> [backend\_protocol](#input\_backend\_protocol)

Description: The protocol the EKS cluster.

Type: `string`

Default: `"TCP"`

### <a name="input_bastion_instance_type"></a> [bastion\_instance\_type](#input\_bastion\_instance\_type)

Description: Instance type for Bastion

Type: `string`

Default: `"t3a.micro"`

### <a name="input_branch"></a> [branch](#input\_branch)

Description: Branch from which code was deployed, develop or master.

Type: `string`

Default: `""`

### <a name="input_dns_domain"></a> [dns\_domain](#input\_dns\_domain)

Description: Precreated domain for project in Route53.

Type: `string`

Default: `"se-tpm.com"`

### <a name="input_dns_fullname_wireguard"></a> [dns\_fullname\_wireguard](#input\_dns\_fullname\_wireguard)

Description: Domain name for VPN Wireguard.

Type: `string`

Default: `"wireguard.se-tpm.com"`

### <a name="input_dynamodb_backup"></a> [dynamodb\_backup](#input\_dynamodb\_backup)

Description: Backup retention for dynamodb.

Type: `number`

Default: `7`

### <a name="input_eks_instance_type"></a> [eks\_instance\_type](#input\_eks\_instance\_type)

Description: EKS instance type

Type: `string`

Default: `"t3a.large"`

### <a name="input_eks_node_ami"></a> [eks\_node\_ami](#input\_eks\_node\_ami)

Description: EKS nodes AMI versions map, to fix EKS node version.

Type: `map`

Default:

```json
{
  "ap-northeast-1": "ami-022b7082336a35fa5",
  "ap-northeast-2": "ami-00e09b556bc0a5250",
  "ap-south-1": "ami-02116767eec13d483",
  "ap-southeast-1": "ami-0c5b93563fd4c0b64",
  "ap-southeast-2": "ami-0fdce91f54abc819c",
  "ca-central-1": "ami-07f84ec952ff04c55",
  "eu-central-1": "ami-0b63408a8fdf0dfbb",
  "eu-north-1": "ami-07852cbef6938d8d4",
  "eu-west-1": "ami-072fbef2a16895c26",
  "eu-west-3": "ami-063dde54d493f0b10",
  "sa-east-1": "ami-0edf89f8165ab8929",
  "us-east-1": "ami-09d01d46812c52d7d",
  "us-east-2": "ami-0a8371504b52964aa",
  "us-west-1": "ami-0d8c692eebb0c2b85",
  "us-west-2": "ami-09f3859628fa7c789"
}
```

### <a name="input_eks_version"></a> [eks\_version](#input\_eks\_version)

Description: EKS version

Type: `string`

Default: `"1.20"`

### <a name="input_elasticsearch_automated_snapshot_start_hour"></a> [elasticsearch\_automated\_snapshot\_start\_hour](#input\_elasticsearch\_automated\_snapshot\_start\_hour)

Description: Elasticsearch automated\_snapshot\_start\_hour

Type: `string`

Default: `"23"`

### <a name="input_elasticsearch_availability_zone_count"></a> [elasticsearch\_availability\_zone\_count](#input\_elasticsearch\_availability\_zone\_count)

Description: Elasticsearch availability zone count

Type: `string`

Default: `"3"`

### <a name="input_elasticsearch_domain_name"></a> [elasticsearch\_domain\_name](#input\_elasticsearch\_domain\_name)

Description: Elasticsearch domain name.

Type: `string`

Default: `"setpm-logs"`

### <a name="input_elasticsearch_ebs_volume_size_apps_logs"></a> [elasticsearch\_ebs\_volume\_size\_apps\_logs](#input\_elasticsearch\_ebs\_volume\_size\_apps\_logs)

Description: Elasticsearch EBS volume size

Type: `string`

Default: `"35"`

### <a name="input_elasticsearch_ebs_volume_size_apps_statistic"></a> [elasticsearch\_ebs\_volume\_size\_apps\_statistic](#input\_elasticsearch\_ebs\_volume\_size\_apps\_statistic)

Description: Elasticsearch EBS volume size

Type: `string`

Default: `"20"`

### <a name="input_elasticsearch_instance_count"></a> [elasticsearch\_instance\_count](#input\_elasticsearch\_instance\_count)

Description: Elasticsearch instance count

Type: `string`

Default: `"3"`

### <a name="input_elasticsearch_instance_type_apps_logs"></a> [elasticsearch\_instance\_type\_apps\_logs](#input\_elasticsearch\_instance\_type\_apps\_logs)

Description: Elasticsearch instance type

Type: `string`

Default: `"t3.medium.elasticsearch"`

### <a name="input_elasticsearch_instance_type_apps_statistic"></a> [elasticsearch\_instance\_type\_apps\_statistic](#input\_elasticsearch\_instance\_type\_apps\_statistic)

Description: Elasticsearch instance type

Type: `string`

Default: `"t3.small.elasticsearch"`

### <a name="input_elasticsearch_version"></a> [elasticsearch\_version](#input\_elasticsearch\_version)

Description: Elasticsearch version

Type: `string`

Default: `"6.8"`

### <a name="input_firebase_token"></a> [firebase\_token](#input\_firebase\_token)

Description: SNS/Platform applications/FCM token for Firebase (FCM) connection.

Type: `string`

Default: `"AAAAKxyqu78:APA91bGnn9-xp7Ev5Yr_T3AuHdlWbjV-a6I7AjhM3tPI_P42sh-V65iP17aPqdQ3rByZZjVpfKUiDOUO5JiMxAmwIezzF2VIGT86nVz_bb7-3xlJzgua2f2o5lhPL4O9Tbcpu_b41Ws1"`

### <a name="input_image_tag"></a> [image\_tag](#input\_image\_tag)

Description: Image tag

Type: `string`

Default: `"develop"`

### <a name="input_iot_se_commands"></a> [iot\_se\_commands](#input\_iot\_se\_commands)

Description: IOT se commands

Type: `string`

Default: `"/v1/se/commands/"`

### <a name="input_iot_se_events"></a> [iot\_se\_events](#input\_iot\_se\_events)

Description: IOT se events

Type: `string`

Default: `"/v1/se/events/"`

### <a name="input_ipsubnet_extaccess"></a> [ipsubnet\_extaccess](#input\_ipsubnet\_extaccess)

Description: External network origins to accept access.

Type: `list`

Default:

```json
[
  "195.234.74.0/24",
  "195.238.93.0/24",
  "195.238.93.128/32",
  "34.89.223.156/32",
  "83.23.238.209/32",
  "46.219.224.0/24",
  "95.215.159.102/32",
  "92.253.236.242/32",
  "176.104.1.114/32",
  "188.239.63.103/32",
  "89.22.205.90/32",
  "24.34.49.120/32",
  "71.131.67.132/32",
  "109.196.42.90/32"
]
```

### <a name="input_kubectl_path"></a> [kubectl\_path](#input\_kubectl\_path)

Description: local path to kubectl binary.

Type: `string`

Default: `""`

### <a name="input_mail_sender_address"></a> [mail\_sender\_address](#input\_mail\_sender\_address)

Description: Email sender address. Note: should be manually varified in AWS SES service.

Type: `string`

Default: `"tsm.portal.lite@gmail.com"`

### <a name="input_openldap_admin_user"></a> [openldap\_admin\_user](#input\_openldap\_admin\_user)

Description: Administrator user for OpenLDAP.

Type: `string`

Default: `"admin"`

### <a name="input_openldap_instance_type"></a> [openldap\_instance\_type](#input\_openldap\_instance\_type)

Description: openldap instance type

Type: `string`

Default: `"t3a.micro"`

### <a name="input_ssh_key"></a> [ssh\_key](#input\_ssh\_key)

Description: SSH-key for EC2.

Type: `string`

Default: `"globallogic-tpm"`

### <a name="input_tags"></a> [tags](#input\_tags)

Description: Default tags set.

Type: `map`

Default:

```json
{
  "Creator": "GL-DevOpsTeam",
  "Environment": "develop",
  "Project": "SETPM",
  "Release": "1.0"
}
```

### <a name="input_target_type"></a> [target\_type](#input\_target\_type)

Description: The type of target

Type: `string`

Default: `"instance"`

### <a name="input_vpc_cidr_starting_ip"></a> [vpc\_cidr\_starting\_ip](#input\_vpc\_cidr\_starting\_ip)

Description: This value will serve as the starting IP for a /16 CIDR. Example: a value of 10.0.0.0 will result in CIDR 10.0.0.0/16.

Type: `string`

Default: `"101.101.0.0"`
## Modules

No modules.
## Outputs

The following outputs are exported:

### <a name="output_AWS_CERT_BUCKET_NAME"></a> [AWS\_CERT\_BUCKET\_NAME](#output\_AWS\_CERT\_BUCKET\_NAME)

Description: n/a

### <a name="output_DYNAMO_APIKEY_CS_TABLE"></a> [DYNAMO\_APIKEY\_CS\_TABLE](#output\_DYNAMO\_APIKEY\_CS\_TABLE)

Description: n/a

### <a name="output_DYNAMO_APIKEY_DG_TABLE"></a> [DYNAMO\_APIKEY\_DG\_TABLE](#output\_DYNAMO\_APIKEY\_DG\_TABLE)

Description: n/a

### <a name="output_DYNAMO_APIKEY_TABLE"></a> [DYNAMO\_APIKEY\_TABLE](#output\_DYNAMO\_APIKEY\_TABLE)

Description: vsts-user-service

### <a name="output_DYNAMO_APPLET_TABLE"></a> [DYNAMO\_APPLET\_TABLE](#output\_DYNAMO\_APPLET\_TABLE)

Description: n/a

### <a name="output_DYNAMO_BS_ICCID_INFO_TABLE"></a> [DYNAMO\_BS\_ICCID\_INFO\_TABLE](#output\_DYNAMO\_BS\_ICCID\_INFO\_TABLE)

Description: n/a

### <a name="output_DYNAMO_CAMPAIGN_EXECUTION_TABLE_CAMPAIGN_ORCHESTARTOR"></a> [DYNAMO\_CAMPAIGN\_EXECUTION\_TABLE\_CAMPAIGN\_ORCHESTARTOR](#output\_DYNAMO\_CAMPAIGN\_EXECUTION\_TABLE\_CAMPAIGN\_ORCHESTARTOR)

Description: n/a

### <a name="output_DYNAMO_CAMPAIGN_EXECUTION_TABLE_CONTENT_SERVICE"></a> [DYNAMO\_CAMPAIGN\_EXECUTION\_TABLE\_CONTENT\_SERVICE](#output\_DYNAMO\_CAMPAIGN\_EXECUTION\_TABLE\_CONTENT\_SERVICE)

Description: n/a

### <a name="output_DYNAMO_CAMPAIGN_TABLE"></a> [DYNAMO\_CAMPAIGN\_TABLE](#output\_DYNAMO\_CAMPAIGN\_TABLE)

Description: n/a

### <a name="output_DYNAMO_COMMAND_EXECUTION_TABLE"></a> [DYNAMO\_COMMAND\_EXECUTION\_TABLE](#output\_DYNAMO\_COMMAND\_EXECUTION\_TABLE)

Description: n/a

### <a name="output_DYNAMO_COMMAND_PREPARATION_TABLE"></a> [DYNAMO\_COMMAND\_PREPARATION\_TABLE](#output\_DYNAMO\_COMMAND\_PREPARATION\_TABLE)

Description: n/a

### <a name="output_DYNAMO_COMMAND_PREPARATION_TABLE_GP"></a> [DYNAMO\_COMMAND\_PREPARATION\_TABLE\_GP](#output\_DYNAMO\_COMMAND\_PREPARATION\_TABLE\_GP)

Description: n/a

### <a name="output_DYNAMO_CS_SCRIPT_EXECUTION"></a> [DYNAMO\_CS\_SCRIPT\_EXECUTION](#output\_DYNAMO\_CS\_SCRIPT\_EXECUTION)

Description: vsts-lambda-db-campaign-execution

### <a name="output_DYNAMO_CUSTOM_COMMANDS_TABLE"></a> [DYNAMO\_CUSTOM\_COMMANDS\_TABLE](#output\_DYNAMO\_CUSTOM\_COMMANDS\_TABLE)

Description: n/a

### <a name="output_DYNAMO_DEVICE_COMMAND_TABLE"></a> [DYNAMO\_DEVICE\_COMMAND\_TABLE](#output\_DYNAMO\_DEVICE\_COMMAND\_TABLE)

Description: n/a

### <a name="output_DYNAMO_DEVICE_CONFIG_LINKS"></a> [DYNAMO\_DEVICE\_CONFIG\_LINKS](#output\_DYNAMO\_DEVICE\_CONFIG\_LINKS)

Description: n/a

### <a name="output_DYNAMO_DEVICE_INFO_TABLE"></a> [DYNAMO\_DEVICE\_INFO\_TABLE](#output\_DYNAMO\_DEVICE\_INFO\_TABLE)

Description: n/a

### <a name="output_DYNAMO_DEVICE_NOTIFICATIONS_TABLE"></a> [DYNAMO\_DEVICE\_NOTIFICATIONS\_TABLE](#output\_DYNAMO\_DEVICE\_NOTIFICATIONS\_TABLE)

Description: n/a

### <a name="output_DYNAMO_DG_VENDOR_TABLE"></a> [DYNAMO\_DG\_VENDOR\_TABLE](#output\_DYNAMO\_DG\_VENDOR\_TABLE)

Description: n/a

### <a name="output_DYNAMO_GROUPED_COMMANDS_TABLE"></a> [DYNAMO\_GROUPED\_COMMANDS\_TABLE](#output\_DYNAMO\_GROUPED\_COMMANDS\_TABLE)

Description: n/a

### <a name="output_DYNAMO_ICCID_RELATIONS_TABLE_SK_PK_INDEX"></a> [DYNAMO\_ICCID\_RELATIONS\_TABLE\_SK\_PK\_INDEX](#output\_DYNAMO\_ICCID\_RELATIONS\_TABLE\_SK\_PK\_INDEX)

Description: n/a

### <a name="output_DYNAMO_KS_ICCID_INFO"></a> [DYNAMO\_KS\_ICCID\_INFO](#output\_DYNAMO\_KS\_ICCID\_INFO)

Description: n/a

### <a name="output_DYNAMO_RELATION_PROFILE_TABLE"></a> [DYNAMO\_RELATION\_PROFILE\_TABLE](#output\_DYNAMO\_RELATION\_PROFILE\_TABLE)

Description: n/a

### <a name="output_DYNAMO_RELATION_PROFILE_TABLE_NAME_SCRIPT_ID_INDEX"></a> [DYNAMO\_RELATION\_PROFILE\_TABLE\_NAME\_SCRIPT\_ID\_INDEX](#output\_DYNAMO\_RELATION\_PROFILE\_TABLE\_NAME\_SCRIPT\_ID\_INDEX)

Description: n/a

### <a name="output_DYNAMO_ROLE_TABLE"></a> [DYNAMO\_ROLE\_TABLE](#output\_DYNAMO\_ROLE\_TABLE)

Description: n/a

### <a name="output_DYNAMO_SCHEDULED_EVENT_TABLE"></a> [DYNAMO\_SCHEDULED\_EVENT\_TABLE](#output\_DYNAMO\_SCHEDULED\_EVENT\_TABLE)

Description: vsts-event-scheduler

### <a name="output_DYNAMO_SCRIPT_EXECUTION_TABLE_CAMPAIGN_ORCHESTRATOR"></a> [DYNAMO\_SCRIPT\_EXECUTION\_TABLE\_CAMPAIGN\_ORCHESTRATOR](#output\_DYNAMO\_SCRIPT\_EXECUTION\_TABLE\_CAMPAIGN\_ORCHESTRATOR)

Description: vsts-campaign-orchestrator

### <a name="output_DYNAMO_SCRIPT_EXECUTION_TABLE_CONTENT_SERVICE"></a> [DYNAMO\_SCRIPT\_EXECUTION\_TABLE\_CONTENT\_SERVICE](#output\_DYNAMO\_SCRIPT\_EXECUTION\_TABLE\_CONTENT\_SERVICE)

Description: n/a

### <a name="output_DYNAMO_SCRIPT_TABLE"></a> [DYNAMO\_SCRIPT\_TABLE](#output\_DYNAMO\_SCRIPT\_TABLE)

Description: n/a

### <a name="output_DYNAMO_SCRIPT_TABLE_SRV_SCRIPT_EXECUTOR"></a> [DYNAMO\_SCRIPT\_TABLE\_SRV\_SCRIPT\_EXECUTOR](#output\_DYNAMO\_SCRIPT\_TABLE\_SRV\_SCRIPT\_EXECUTOR)

Description: n/a

### <a name="output_DYNAMO_SCRIPT_TEMPLATE_TABLE"></a> [DYNAMO\_SCRIPT\_TEMPLATE\_TABLE](#output\_DYNAMO\_SCRIPT\_TEMPLATE\_TABLE)

Description: n/a

### <a name="output_DYNAMO_SCRIPT_TEMPLATE_TABLE_NAME_VENDOR_ID_INDEX"></a> [DYNAMO\_SCRIPT\_TEMPLATE\_TABLE\_NAME\_VENDOR\_ID\_INDEX](#output\_DYNAMO\_SCRIPT\_TEMPLATE\_TABLE\_NAME\_VENDOR\_ID\_INDEX)

Description: n/a

### <a name="output_DYNAMO_SUPPORTED_CA_TABLE"></a> [DYNAMO\_SUPPORTED\_CA\_TABLE](#output\_DYNAMO\_SUPPORTED\_CA\_TABLE)

Description: n/a

### <a name="output_DYNAMO_SUPPORTED_COMMANDS_TABLE"></a> [DYNAMO\_SUPPORTED\_COMMANDS\_TABLE](#output\_DYNAMO\_SUPPORTED\_COMMANDS\_TABLE)

Description: n/a

### <a name="output_DYNAMO_TABLE_GP_APPLET"></a> [DYNAMO\_TABLE\_GP\_APPLET](#output\_DYNAMO\_TABLE\_GP\_APPLET)

Description: n/a

### <a name="output_DYNAMO_TABLE_ICCID"></a> [DYNAMO\_TABLE\_ICCID](#output\_DYNAMO\_TABLE\_ICCID)

Description: n/a

### <a name="output_DYNAMO_TABLE_IDENTITIES"></a> [DYNAMO\_TABLE\_IDENTITIES](#output\_DYNAMO\_TABLE\_IDENTITIES)

Description: n/a

### <a name="output_DYNAMO_UICC_GROUP_TABLE"></a> [DYNAMO\_UICC\_GROUP\_TABLE](#output\_DYNAMO\_UICC\_GROUP\_TABLE)

Description: n/a

### <a name="output_DYNAMO_UICC_STATUS_INDEX_NAME"></a> [DYNAMO\_UICC\_STATUS\_INDEX\_NAME](#output\_DYNAMO\_UICC\_STATUS\_INDEX\_NAME)

Description: n/a

### <a name="output_DYNAMO_UICC_TABLE"></a> [DYNAMO\_UICC\_TABLE](#output\_DYNAMO\_UICC\_TABLE)

Description: n/a

### <a name="output_DYNAMO_USER_INFO_TABLE"></a> [DYNAMO\_USER\_INFO\_TABLE](#output\_DYNAMO\_USER\_INFO\_TABLE)

Description: n/a

### <a name="output_DYNAMO_USER_TABLE"></a> [DYNAMO\_USER\_TABLE](#output\_DYNAMO\_USER\_TABLE)

Description: n/a

### <a name="output_DYNAMO_VENDOR_INFO_TABLE"></a> [DYNAMO\_VENDOR\_INFO\_TABLE](#output\_DYNAMO\_VENDOR\_INFO\_TABLE)

Description: n/a

### <a name="output_DYNAMO_VENDOR_PERMISSIONS_TABLE"></a> [DYNAMO\_VENDOR\_PERMISSIONS\_TABLE](#output\_DYNAMO\_VENDOR\_PERMISSIONS\_TABLE)

Description: n/a

### <a name="output_DYNAMO_VENDOR_TABLE"></a> [DYNAMO\_VENDOR\_TABLE](#output\_DYNAMO\_VENDOR\_TABLE)

Description: n/a

### <a name="output_IOT_BROKER_URL"></a> [IOT\_BROKER\_URL](#output\_IOT\_BROKER\_URL)

Description: n/a

### <a name="output_PROXY_APPLET_COMMAND_TABLE"></a> [PROXY\_APPLET\_COMMAND\_TABLE](#output\_PROXY\_APPLET\_COMMAND\_TABLE)

Description: n/a

### <a name="output_PROXY_APPLET_COMMAND_TABLE_INDEX"></a> [PROXY\_APPLET\_COMMAND\_TABLE\_INDEX](#output\_PROXY\_APPLET\_COMMAND\_TABLE\_INDEX)

Description: n/a

### <a name="output_PROXY_APPLET_SESSION_INFO"></a> [PROXY\_APPLET\_SESSION\_INFO](#output\_PROXY\_APPLET\_SESSION\_INFO)

Description: n/a

### <a name="output_SE_DEVICE_INFO_QUEUE"></a> [SE\_DEVICE\_INFO\_QUEUE](#output\_SE\_DEVICE\_INFO\_QUEUE)

Description: n/a

### <a name="output_SE_DEVICE_INFO_TABLE"></a> [SE\_DEVICE\_INFO\_TABLE](#output\_SE\_DEVICE\_INFO\_TABLE)

Description: n/a

### <a name="output_SNS_CA_CERT_GEN_TOPIC"></a> [SNS\_CA\_CERT\_GEN\_TOPIC](#output\_SNS\_CA\_CERT\_GEN\_TOPIC)

Description: n/a

### <a name="output_SNS_CA_COMMANDS"></a> [SNS\_CA\_COMMANDS](#output\_SNS\_CA\_COMMANDS)

Description: n/a

### <a name="output_SNS_CA_EVENTS_TOPIC"></a> [SNS\_CA\_EVENTS\_TOPIC](#output\_SNS\_CA\_EVENTS\_TOPIC)

Description: n/a

### <a name="output_SNS_CHANNEL_APPLET_EVENTS"></a> [SNS\_CHANNEL\_APPLET\_EVENTS](#output\_SNS\_CHANNEL\_APPLET\_EVENTS)

Description: n/a

### <a name="output_SNS_CHANNEL_BOOTSTRAP_EVENTS"></a> [SNS\_CHANNEL\_BOOTSTRAP\_EVENTS](#output\_SNS\_CHANNEL\_BOOTSTRAP\_EVENTS)

Description: vsts-bootstrap-service

### <a name="output_SNS_CHANNEL_CAMPAIGN_COMMANDS"></a> [SNS\_CHANNEL\_CAMPAIGN\_COMMANDS](#output\_SNS\_CHANNEL\_CAMPAIGN\_COMMANDS)

Description: vsts-content-service

### <a name="output_SNS_CHANNEL_CAMPAIGN_EVENTS"></a> [SNS\_CHANNEL\_CAMPAIGN\_EVENTS](#output\_SNS\_CHANNEL\_CAMPAIGN\_EVENTS)

Description: n/a

### <a name="output_SNS_CHANNEL_CAMPAIGN_EVENTS_ARN"></a> [SNS\_CHANNEL\_CAMPAIGN\_EVENTS\_ARN](#output\_SNS\_CHANNEL\_CAMPAIGN\_EVENTS\_ARN)

Description: n/a

### <a name="output_SNS_CHANNEL_CRYPTO_EVENTS"></a> [SNS\_CHANNEL\_CRYPTO\_EVENTS](#output\_SNS\_CHANNEL\_CRYPTO\_EVENTS)

Description: n/a

### <a name="output_SNS_CHANNEL_CRYPTO_SERVICE_EVENTS"></a> [SNS\_CHANNEL\_CRYPTO\_SERVICE\_EVENTS](#output\_SNS\_CHANNEL\_CRYPTO\_SERVICE\_EVENTS)

Description: n/a

### <a name="output_SNS_CHANNEL_DEVICE_NOTIFICATIONS"></a> [SNS\_CHANNEL\_DEVICE\_NOTIFICATIONS](#output\_SNS\_CHANNEL\_DEVICE\_NOTIFICATIONS)

Description: vsts-notification-service

### <a name="output_SNS_CHANNEL_GP_CRYPTO_EVENTS"></a> [SNS\_CHANNEL\_GP\_CRYPTO\_EVENTS](#output\_SNS\_CHANNEL\_GP\_CRYPTO\_EVENTS)

Description: n/a

### <a name="output_SNS_CHANNEL_PROXY_APPLET_DEVICE_COMMANDS"></a> [SNS\_CHANNEL\_PROXY\_APPLET\_DEVICE\_COMMANDS](#output\_SNS\_CHANNEL\_PROXY\_APPLET\_DEVICE\_COMMANDS)

Description: vsts-proxy-applet-service

### <a name="output_SNS_CHANNEL_SCHEDULED_EVENTS"></a> [SNS\_CHANNEL\_SCHEDULED\_EVENTS](#output\_SNS\_CHANNEL\_SCHEDULED\_EVENTS)

Description: n/a

### <a name="output_SNS_CHANNEL_SCRIPT_COMMANDS"></a> [SNS\_CHANNEL\_SCRIPT\_COMMANDS](#output\_SNS\_CHANNEL\_SCRIPT\_COMMANDS)

Description: n/a

### <a name="output_SNS_CHANNEL_STATISTIC_TOPIC"></a> [SNS\_CHANNEL\_STATISTIC\_TOPIC](#output\_SNS\_CHANNEL\_STATISTIC\_TOPIC)

Description: n/a

### <a name="output_SNS_CHANNEL_USER_COMMANDS"></a> [SNS\_CHANNEL\_USER\_COMMANDS](#output\_SNS\_CHANNEL\_USER\_COMMANDS)

Description: n/a

### <a name="output_SNS_CHANNEL_USER_EVENTS"></a> [SNS\_CHANNEL\_USER\_EVENTS](#output\_SNS\_CHANNEL\_USER\_EVENTS)

Description: n/a

### <a name="output_SNS_CI_COMMANDS_TOPIC"></a> [SNS\_CI\_COMMANDS\_TOPIC](#output\_SNS\_CI\_COMMANDS\_TOPIC)

Description: n/a

### <a name="output_SNS_CI_EVENTS_TOPIC"></a> [SNS\_CI\_EVENTS\_TOPIC](#output\_SNS\_CI\_EVENTS\_TOPIC)

Description: vsts-ci-service

### <a name="output_SNS_COMMAND_EVENTS_TOPIC"></a> [SNS\_COMMAND\_EVENTS\_TOPIC](#output\_SNS\_COMMAND\_EVENTS\_TOPIC)

Description: n/a

### <a name="output_SNS_CRYPTO_COMMANDS_TOPIC"></a> [SNS\_CRYPTO\_COMMANDS\_TOPIC](#output\_SNS\_CRYPTO\_COMMANDS\_TOPIC)

Description: n/a

### <a name="output_SNS_DEVICE_COMMANDS_TOPIC"></a> [SNS\_DEVICE\_COMMANDS\_TOPIC](#output\_SNS\_DEVICE\_COMMANDS\_TOPIC)

Description: n/a

### <a name="output_SNS_DEVICE_EVENTS_TOPIC"></a> [SNS\_DEVICE\_EVENTS\_TOPIC](#output\_SNS\_DEVICE\_EVENTS\_TOPIC)

Description: vsts-device-gateway

### <a name="output_SNS_DEVICE_INFO_TOPIC"></a> [SNS\_DEVICE\_INFO\_TOPIC](#output\_SNS\_DEVICE\_INFO\_TOPIC)

Description: n/a

### <a name="output_SNS_GP_CI_EVENTS_TOPIC"></a> [SNS\_GP\_CI\_EVENTS\_TOPIC](#output\_SNS\_GP\_CI\_EVENTS\_TOPIC)

Description: n/a

### <a name="output_SNS_GP_COMMANDS_TOPIC"></a> [SNS\_GP\_COMMANDS\_TOPIC](#output\_SNS\_GP\_COMMANDS\_TOPIC)

Description: n/a

### <a name="output_SNS_KCSS_COMMANDS_TOPIC"></a> [SNS\_KCSS\_COMMANDS\_TOPIC](#output\_SNS\_KCSS\_COMMANDS\_TOPIC)

Description: n/a

### <a name="output_SNS_KEYS_COMMANDS"></a> [SNS\_KEYS\_COMMANDS](#output\_SNS\_KEYS\_COMMANDS)

Description: n/a

### <a name="output_SNS_KEYS_EVENTS"></a> [SNS\_KEYS\_EVENTS](#output\_SNS\_KEYS\_EVENTS)

Description: n/a

### <a name="output_SNS_KEY_SERVICE_COMMANDS"></a> [SNS\_KEY\_SERVICE\_COMMANDS](#output\_SNS\_KEY\_SERVICE\_COMMANDS)

Description: n/a

### <a name="output_SNS_PROXY_APPLET_COMMANDS"></a> [SNS\_PROXY\_APPLET\_COMMANDS](#output\_SNS\_PROXY\_APPLET\_COMMANDS)

Description: n/a

### <a name="output_SNS_PUSH_NOTIFICATION_ARN"></a> [SNS\_PUSH\_NOTIFICATION\_ARN](#output\_SNS\_PUSH\_NOTIFICATION\_ARN)

Description: n/a

### <a name="output_SNS_SCRIPT_COMMANDS_SUPPORTED_TOPIC"></a> [SNS\_SCRIPT\_COMMANDS\_SUPPORTED\_TOPIC](#output\_SNS\_SCRIPT\_COMMANDS\_SUPPORTED\_TOPIC)

Description: n/a

### <a name="output_SNS_SCRIPT_EVENTS_TOPIC"></a> [SNS\_SCRIPT\_EVENTS\_TOPIC](#output\_SNS\_SCRIPT\_EVENTS\_TOPIC)

Description: n/a

### <a name="output_SNS_STATISTICS_EVENTS"></a> [SNS\_STATISTICS\_EVENTS](#output\_SNS\_STATISTICS\_EVENTS)

Description: n/a

### <a name="output_SNS_SUPPORTED_COMMANDS_TOPIC"></a> [SNS\_SUPPORTED\_COMMANDS\_TOPIC](#output\_SNS\_SUPPORTED\_COMMANDS\_TOPIC)

Description: vsts-kcss-service

### <a name="output_SNS_TOPIC_PREFIX"></a> [SNS\_TOPIC\_PREFIX](#output\_SNS\_TOPIC\_PREFIX)

Description: n/a

### <a name="output_SNS_UICC"></a> [SNS\_UICC](#output\_SNS\_UICC)

Description: n/a

### <a name="output_SQS_CA_CERT_GEN_QUEUE"></a> [SQS\_CA\_CERT\_GEN\_QUEUE](#output\_SQS\_CA\_CERT\_GEN\_QUEUE)

Description: n/a

### <a name="output_SQS_CA_COMMANDS"></a> [SQS\_CA\_COMMANDS](#output\_SQS\_CA\_COMMANDS)

Description: n/a

### <a name="output_SQS_CHANNEL_APPLET_EVENTS"></a> [SQS\_CHANNEL\_APPLET\_EVENTS](#output\_SQS\_CHANNEL\_APPLET\_EVENTS)

Description: n/a

### <a name="output_SQS_CHANNEL_BOOTSTRAP_EVENTS"></a> [SQS\_CHANNEL\_BOOTSTRAP\_EVENTS](#output\_SQS\_CHANNEL\_BOOTSTRAP\_EVENTS)

Description: n/a

### <a name="output_SQS_CHANNEL_CAMPAIGN_COMMANDS"></a> [SQS\_CHANNEL\_CAMPAIGN\_COMMANDS](#output\_SQS\_CHANNEL\_CAMPAIGN\_COMMANDS)

Description: n/a

### <a name="output_SQS_CHANNEL_CAMPAIGN_EVENTS"></a> [SQS\_CHANNEL\_CAMPAIGN\_EVENTS](#output\_SQS\_CHANNEL\_CAMPAIGN\_EVENTS)

Description: n/a

### <a name="output_SQS_CHANNEL_CA_EVENTS"></a> [SQS\_CHANNEL\_CA\_EVENTS](#output\_SQS\_CHANNEL\_CA\_EVENTS)

Description: n/a

### <a name="output_SQS_CHANNEL_CRYPTO_COMMANDS"></a> [SQS\_CHANNEL\_CRYPTO\_COMMANDS](#output\_SQS\_CHANNEL\_CRYPTO\_COMMANDS)

Description: vsts-crypto-service

### <a name="output_SQS_CHANNEL_DEVICE_NOTIFICATIONS"></a> [SQS\_CHANNEL\_DEVICE\_NOTIFICATIONS](#output\_SQS\_CHANNEL\_DEVICE\_NOTIFICATIONS)

Description: n/a

### <a name="output_SQS_CHANNEL_GENERIC_EVENTS"></a> [SQS\_CHANNEL\_GENERIC\_EVENTS](#output\_SQS\_CHANNEL\_GENERIC\_EVENTS)

Description: n/a

### <a name="output_SQS_CHANNEL_GP_CRYPTO_EVENTS"></a> [SQS\_CHANNEL\_GP\_CRYPTO\_EVENTS](#output\_SQS\_CHANNEL\_GP\_CRYPTO\_EVENTS)

Description: n/a

### <a name="output_SQS_CHANNEL_ICCID_EVENTS"></a> [SQS\_CHANNEL\_ICCID\_EVENTS](#output\_SQS\_CHANNEL\_ICCID\_EVENTS)

Description: n/a

### <a name="output_SQS_CHANNEL_KS_UICC"></a> [SQS\_CHANNEL\_KS\_UICC](#output\_SQS\_CHANNEL\_KS\_UICC)

Description: n/a

### <a name="output_SQS_CHANNEL_PROXY_APPLET_DEVICE_COMMAND_EVENTS"></a> [SQS\_CHANNEL\_PROXY\_APPLET\_DEVICE\_COMMAND\_EVENTS](#output\_SQS\_CHANNEL\_PROXY\_APPLET\_DEVICE\_COMMAND\_EVENTS)

Description: n/a

### <a name="output_SQS_CHANNEL_SCHEDULED_EVENTS_COMMANDS"></a> [SQS\_CHANNEL\_SCHEDULED\_EVENTS\_COMMANDS](#output\_SQS\_CHANNEL\_SCHEDULED\_EVENTS\_COMMANDS)

Description: n/a

### <a name="output_SQS_CHANNEL_SCRIPT_EVENTS"></a> [SQS\_CHANNEL\_SCRIPT\_EVENTS](#output\_SQS\_CHANNEL\_SCRIPT\_EVENTS)

Description: n/a

### <a name="output_SQS_CHANNEL_SECURE_MESSAGING_EVENTS"></a> [SQS\_CHANNEL\_SECURE\_MESSAGING\_EVENTS](#output\_SQS\_CHANNEL\_SECURE\_MESSAGING\_EVENTS)

Description: n/a

### <a name="output_SQS_CHANNEL_STATISTIC_QUEUE"></a> [SQS\_CHANNEL\_STATISTIC\_QUEUE](#output\_SQS\_CHANNEL\_STATISTIC\_QUEUE)

Description: vsts-statistic-service

### <a name="output_SQS_CHANNEL_SUPPORTED_COMMANDS_EVENTS"></a> [SQS\_CHANNEL\_SUPPORTED\_COMMANDS\_EVENTS](#output\_SQS\_CHANNEL\_SUPPORTED\_COMMANDS\_EVENTS)

Description: n/a

### <a name="output_SQS_CHANNEL_USER_COMMANDS"></a> [SQS\_CHANNEL\_USER\_COMMANDS](#output\_SQS\_CHANNEL\_USER\_COMMANDS)

Description: n/a

### <a name="output_SQS_CHANNEL_USER_EVENTS"></a> [SQS\_CHANNEL\_USER\_EVENTS](#output\_SQS\_CHANNEL\_USER\_EVENTS)

Description: n/a

### <a name="output_SQS_CHANNEL_VENDOR_CO_EVENTS"></a> [SQS\_CHANNEL\_VENDOR\_CO\_EVENTS](#output\_SQS\_CHANNEL\_VENDOR\_CO\_EVENTS)

Description: n/a

### <a name="output_SQS_CHANNEL_VENDOR_EVENTS"></a> [SQS\_CHANNEL\_VENDOR\_EVENTS](#output\_SQS\_CHANNEL\_VENDOR\_EVENTS)

Description: n/a

### <a name="output_SQS_CI_COMMANDS_QUEUE"></a> [SQS\_CI\_COMMANDS\_QUEUE](#output\_SQS\_CI\_COMMANDS\_QUEUE)

Description: n/a

### <a name="output_SQS_CI_EVENTS_QUEUE"></a> [SQS\_CI\_EVENTS\_QUEUE](#output\_SQS\_CI\_EVENTS\_QUEUE)

Description: common with script-executor-service

### <a name="output_SQS_COMMAND_EVENTS_QUEUE"></a> [SQS\_COMMAND\_EVENTS\_QUEUE](#output\_SQS\_COMMAND\_EVENTS\_QUEUE)

Description: n/a

### <a name="output_SQS_CRYPTO_EVENTS_QUEUE"></a> [SQS\_CRYPTO\_EVENTS\_QUEUE](#output\_SQS\_CRYPTO\_EVENTS\_QUEUE)

Description: n/a

### <a name="output_SQS_DEVICE_COMMANDS_QUEUE"></a> [SQS\_DEVICE\_COMMANDS\_QUEUE](#output\_SQS\_DEVICE\_COMMANDS\_QUEUE)

Description: n/a

### <a name="output_SQS_DEVICE_EVENTS_QUEUE"></a> [SQS\_DEVICE\_EVENTS\_QUEUE](#output\_SQS\_DEVICE\_EVENTS\_QUEUE)

Description: n/a

### <a name="output_SQS_DEVICE_INFO_EVENTS"></a> [SQS\_DEVICE\_INFO\_EVENTS](#output\_SQS\_DEVICE\_INFO\_EVENTS)

Description: n/a

### <a name="output_SQS_DEVICE_ONBOARD_QUEUE"></a> [SQS\_DEVICE\_ONBOARD\_QUEUE](#output\_SQS\_DEVICE\_ONBOARD\_QUEUE)

Description: n/a

### <a name="output_SQS_DIM_COMMAND_EVENTS_QUEUE"></a> [SQS\_DIM\_COMMAND\_EVENTS\_QUEUE](#output\_SQS\_DIM\_COMMAND\_EVENTS\_QUEUE)

Description: n/a

### <a name="output_SQS_DIM_DEVICE_EVENTS_QUEUE"></a> [SQS\_DIM\_DEVICE\_EVENTS\_QUEUE](#output\_SQS\_DIM\_DEVICE\_EVENTS\_QUEUE)

Description: n/a

### <a name="output_SQS_GP_CI_EVENTS_QUEUE"></a> [SQS\_GP\_CI\_EVENTS\_QUEUE](#output\_SQS\_GP\_CI\_EVENTS\_QUEUE)

Description: n/a

### <a name="output_SQS_GP_COMMANDS_QUEUE"></a> [SQS\_GP\_COMMANDS\_QUEUE](#output\_SQS\_GP\_COMMANDS\_QUEUE)

Description: n/a

### <a name="output_SQS_KCSS_COMMANDS_QUEUE"></a> [SQS\_KCSS\_COMMANDS\_QUEUE](#output\_SQS\_KCSS\_COMMANDS\_QUEUE)

Description: n/a

### <a name="output_SQS_KEYS_COMMANDS"></a> [SQS\_KEYS\_COMMANDS](#output\_SQS\_KEYS\_COMMANDS)

Description: n/a

### <a name="output_SQS_KEYS_EVENTS"></a> [SQS\_KEYS\_EVENTS](#output\_SQS\_KEYS\_EVENTS)

Description: n/a

### <a name="output_SQS_KEY_SERVICE_EVENTS"></a> [SQS\_KEY\_SERVICE\_EVENTS](#output\_SQS\_KEY\_SERVICE\_EVENTS)

Description: n/a

### <a name="output_SQS_QUEUE_PREFIX"></a> [SQS\_QUEUE\_PREFIX](#output\_SQS\_QUEUE\_PREFIX)

Description: n/a

### <a name="output_SQS_SCRIPT_COMMANDS_QUEUE"></a> [SQS\_SCRIPT\_COMMANDS\_QUEUE](#output\_SQS\_SCRIPT\_COMMANDS\_QUEUE)

Description: vsts-script-executor

### <a name="output_SQS_SE_EVENTS_QUEUE"></a> [SQS\_SE\_EVENTS\_QUEUE](#output\_SQS\_SE\_EVENTS\_QUEUE)

Description: n/a

### <a name="output_SQS_UICC"></a> [SQS\_UICC](#output\_SQS\_UICC)

Description: n/a

### <a name="output_SQS_USER_COMMANDS_QUEUE"></a> [SQS\_USER\_COMMANDS\_QUEUE](#output\_SQS\_USER\_COMMANDS\_QUEUE)

Description: n/a

### <a name="output_SQS_VENDOR_EVENTS_QUEUE"></a> [SQS\_VENDOR\_EVENTS\_QUEUE](#output\_SQS\_VENDOR\_EVENTS\_QUEUE)

Description: n/a

### <a name="output_api_gateway_domain_name"></a> [api\_gateway\_domain\_name](#output\_api\_gateway\_domain\_name)

Description: n/a

### <a name="output_aws_account_id"></a> [aws\_account\_id](#output\_aws\_account\_id)

Description: n/a

### <a name="output_aws_acm_certificate_arn"></a> [aws\_acm\_certificate\_arn](#output\_aws\_acm\_certificate\_arn)

Description: n/a

### <a name="output_aws_campaign_bucket_name"></a> [aws\_campaign\_bucket\_name](#output\_aws\_campaign\_bucket\_name)

Description: n/a

### <a name="output_aws_ecr_region"></a> [aws\_ecr\_region](#output\_aws\_ecr\_region)

Description: n/a

### <a name="output_aws_iot_certificate_cert_thing_backend_client_certificate_pem"></a> [aws\_iot\_certificate\_cert\_thing\_backend\_client\_certificate\_pem](#output\_aws\_iot\_certificate\_cert\_thing\_backend\_client\_certificate\_pem)

Description: n/a

### <a name="output_aws_iot_certificate_cert_thing_backend_client_private_key"></a> [aws\_iot\_certificate\_cert\_thing\_backend\_client\_private\_key](#output\_aws\_iot\_certificate\_cert\_thing\_backend\_client\_private\_key)

Description: n/a

### <a name="output_aws_region"></a> [aws\_region](#output\_aws\_region)

Description: n/a

### <a name="output_aws_s3_backup_bucket"></a> [aws\_s3\_backup\_bucket](#output\_aws\_s3\_backup\_bucket)

Description: n/a

### <a name="output_ca_certificates"></a> [ca\_certificates](#output\_ca\_certificates)

Description: n/a

### <a name="output_dns_domain"></a> [dns\_domain](#output\_dns\_domain)

Description: n/a

### <a name="output_dns_fullname"></a> [dns\_fullname](#output\_dns\_fullname)

Description: n/a

### <a name="output_dns_fullname_frontend"></a> [dns\_fullname\_frontend](#output\_dns\_fullname\_frontend)

Description: n/a

### <a name="output_efs_key_service_dns_name"></a> [efs\_key\_service\_dns\_name](#output\_efs\_key\_service\_dns\_name)

Description: n/a

### <a name="output_efs_key_service_id"></a> [efs\_key\_service\_id](#output\_efs\_key\_service\_id)

Description: n/a

### <a name="output_eks_cluster_endpoint"></a> [eks\_cluster\_endpoint](#output\_eks\_cluster\_endpoint)

Description: n/a

### <a name="output_eks_cluster_name"></a> [eks\_cluster\_name](#output\_eks\_cluster\_name)

Description: n/a

### <a name="output_eks_instance_role_arn"></a> [eks\_instance\_role\_arn](#output\_eks\_instance\_role\_arn)

Description: n/a

### <a name="output_elasticsearch_endpoint"></a> [elasticsearch\_endpoint](#output\_elasticsearch\_endpoint)

Description: n/a

### <a name="output_elasticsearch_endpoint_statistic"></a> [elasticsearch\_endpoint\_statistic](#output\_elasticsearch\_endpoint\_statistic)

Description: n/a

### <a name="output_iam_mail_sender_user_aws_access_key"></a> [iam\_mail\_sender\_user\_aws\_access\_key](#output\_iam\_mail\_sender\_user\_aws\_access\_key)

Description: n/a

### <a name="output_iam_mail_sender_user_aws_secret_key"></a> [iam\_mail\_sender\_user\_aws\_secret\_key](#output\_iam\_mail\_sender\_user\_aws\_secret\_key)

Description: n/a

### <a name="output_image_tag"></a> [image\_tag](#output\_image\_tag)

Description: n/a

### <a name="output_iot_se_commands"></a> [iot\_se\_commands](#output\_iot\_se\_commands)

Description: n/a

### <a name="output_iot_se_events"></a> [iot\_se\_events](#output\_iot\_se\_events)

Description: n/a

### <a name="output_kub_eks_cluster_autoscaler"></a> [kub\_eks\_cluster\_autoscaler](#output\_kub\_eks\_cluster\_autoscaler)

Description: n/a

### <a name="output_kub_lambda-api-gateway_role_arn"></a> [kub\_lambda-api-gateway\_role\_arn](#output\_kub\_lambda-api-gateway\_role\_arn)

Description: n/a

### <a name="output_kub_prometheus_role_arn"></a> [kub\_prometheus\_role\_arn](#output\_kub\_prometheus\_role\_arn)

Description: n/a

### <a name="output_kub_vsts_bootstrap_service_role_arn"></a> [kub\_vsts\_bootstrap\_service\_role\_arn](#output\_kub\_vsts\_bootstrap\_service\_role\_arn)

Description: n/a

### <a name="output_kub_vsts_campaign_orchestrator_role_arn"></a> [kub\_vsts\_campaign\_orchestrator\_role\_arn](#output\_kub\_vsts\_campaign\_orchestrator\_role\_arn)

Description: IAM roles for K8S

### <a name="output_kub_vsts_ci_service_role_arn"></a> [kub\_vsts\_ci\_service\_role\_arn](#output\_kub\_vsts\_ci\_service\_role\_arn)

Description: n/a

### <a name="output_kub_vsts_content_service_role_arn"></a> [kub\_vsts\_content\_service\_role\_arn](#output\_kub\_vsts\_content\_service\_role\_arn)

Description: n/a

### <a name="output_kub_vsts_crypto_service_role_arn"></a> [kub\_vsts\_crypto\_service\_role\_arn](#output\_kub\_vsts\_crypto\_service\_role\_arn)

Description: n/a

### <a name="output_kub_vsts_device_gateway_role_arn"></a> [kub\_vsts\_device\_gateway\_role\_arn](#output\_kub\_vsts\_device\_gateway\_role\_arn)

Description: n/a

### <a name="output_kub_vsts_dim_service_role_arn"></a> [kub\_vsts\_dim\_service\_role\_arn](#output\_kub\_vsts\_dim\_service\_role\_arn)

Description: n/a

### <a name="output_kub_vsts_event_scheduler_role_arn"></a> [kub\_vsts\_event\_scheduler\_role\_arn](#output\_kub\_vsts\_event\_scheduler\_role\_arn)

Description: n/a

### <a name="output_kub_vsts_gp_service_role_arn"></a> [kub\_vsts\_gp\_service\_role\_arn](#output\_kub\_vsts\_gp\_service\_role\_arn)

Description: n/a

### <a name="output_kub_vsts_kcss_service_role_arn"></a> [kub\_vsts\_kcss\_service\_role\_arn](#output\_kub\_vsts\_kcss\_service\_role\_arn)

Description: n/a

### <a name="output_kub_vsts_key_service_role_arn"></a> [kub\_vsts\_key\_service\_role\_arn](#output\_kub\_vsts\_key\_service\_role\_arn)

Description: n/a

### <a name="output_kub_vsts_notification_service_role_arn"></a> [kub\_vsts\_notification\_service\_role\_arn](#output\_kub\_vsts\_notification\_service\_role\_arn)

Description: n/a

### <a name="output_kub_vsts_proxy_applet_service_role_arn"></a> [kub\_vsts\_proxy\_applet\_service\_role\_arn](#output\_kub\_vsts\_proxy\_applet\_service\_role\_arn)

Description: n/a

### <a name="output_kub_vsts_script_executor_role_arn"></a> [kub\_vsts\_script\_executor\_role\_arn](#output\_kub\_vsts\_script\_executor\_role\_arn)

Description: n/a

### <a name="output_kub_vsts_sms_service_role_arn"></a> [kub\_vsts\_sms\_service\_role\_arn](#output\_kub\_vsts\_sms\_service\_role\_arn)

Description: n/a

### <a name="output_kub_vsts_statistic_service_role_arn"></a> [kub\_vsts\_statistic\_service\_role\_arn](#output\_kub\_vsts\_statistic\_service\_role\_arn)

Description: n/a

### <a name="output_kub_vsts_user_service_role_arn"></a> [kub\_vsts\_user\_service\_role\_arn](#output\_kub\_vsts\_user\_service\_role\_arn)

Description: n/a

### <a name="output_lambda_env_dynamo_grouped_commands_table"></a> [lambda\_env\_dynamo\_grouped\_commands\_table](#output\_lambda\_env\_dynamo\_grouped\_commands\_table)

Description: tables for lambda function

### <a name="output_lambda_trigger_dynamodb_table"></a> [lambda\_trigger\_dynamodb\_table](#output\_lambda\_trigger\_dynamodb\_table)

Description: n/a

### <a name="output_mail_sender_address"></a> [mail\_sender\_address](#output\_mail\_sender\_address)

Description: n/a

### <a name="output_namespace"></a> [namespace](#output\_namespace)

Description: n/a

### <a name="output_openldap_admin_passwd"></a> [openldap\_admin\_passwd](#output\_openldap\_admin\_passwd)

Description: n/a

### <a name="output_openldap_ec2_private_ip"></a> [openldap\_ec2\_private\_ip](#output\_openldap\_ec2\_private\_ip)

Description: n/a

### <a name="output_openldap_login"></a> [openldap\_login](#output\_openldap\_login)

Description: n/a

### <a name="output_openldap_partition_suffix"></a> [openldap\_partition\_suffix](#output\_openldap\_partition\_suffix)

Description: n/a

### <a name="output_openldap_url"></a> [openldap\_url](#output\_openldap\_url)

Description: n/a

### <a name="output_policy_thing_backend_client_name"></a> [policy\_thing\_backend\_client\_name](#output\_policy\_thing\_backend\_client\_name)

Description: n/a

### <a name="output_prefix"></a> [prefix](#output\_prefix)

Description: n/a

### <a name="output_projectname"></a> [projectname](#output\_projectname)

Description: n/a

### <a name="output_s3_device_configuration"></a> [s3\_device\_configuration](#output\_s3\_device\_configuration)

Description: n/a

### <a name="output_s3_static_documentation"></a> [s3\_static\_documentation](#output\_s3\_static\_documentation)

Description: n/a

### <a name="output_vpc_cidr_starting_ip"></a> [vpc\_cidr\_starting\_ip](#output\_vpc\_cidr\_starting\_ip)

Description: n/a
## Providers

The following providers are used by this module:

- <a name="provider_archive"></a> [archive](#provider\_archive)

- <a name="provider_aws"></a> [aws](#provider\_aws) (~> 2.7)

- <a name="provider_external"></a> [external](#provider\_external)

- <a name="provider_local"></a> [local](#provider\_local)

- <a name="provider_null"></a> [null](#provider\_null)

- <a name="provider_random"></a> [random](#provider\_random)
## Requirements

The following requirements are needed by this module:

- <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) (>= 0.13.0, <= 0.13.3)

- <a name="requirement_aws"></a> [aws](#requirement\_aws) (~> 2.7)== ## Resources by Type
[cols="a,a,a,a",options="header,autowidth"]
|===
|Name |File |Type |Spec

## Resources-r-aws_api-gateway.tf
- .aws_acm_certificate.api-gateway-cert |(r-aws_api-gateway.tf#750) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/acm_certificate[aws_acm_certificate.api-gateway-cert]
## Resources-r-aws_openldap.tf
- .aws_acm_certificate.openldap |(r-aws_openldap.tf#126) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/acm_certificate[aws_acm_certificate.openldap]
## Resources-r-aws_acm.tf
- .aws_acm_certificate.wildcard |(r-aws_acm.tf#2) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/acm_certificate[aws_acm_certificate.wildcard]
## Resources-r-aws_api-gateway.tf
- .aws_acm_certificate_validation.api-gateway-valid |(r-aws_api-gateway.tf#762) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/acm_certificate_validation[aws_acm_certificate_validation.api-gateway-valid]
## Resources-r-aws_openldap.tf
- .aws_acm_certificate_validation.openldap |(r-aws_openldap.tf#150) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/acm_certificate_validation[aws_acm_certificate_validation.openldap]
## Resources-r-aws_acm.tf
- .aws_acm_certificate_validation.wildcard |(r-aws_acm.tf#13) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/acm_certificate_validation[aws_acm_certificate_validation.wildcard]
## Resources-r-aws_api-gateway.tf
- .aws_api_gateway_authorizer.lambda-authorizer |(r-aws_api-gateway.tf#846) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_authorizer[aws_api_gateway_authorizer.lambda-authorizer]
- .aws_api_gateway_base_path_mapping.dev |(r-aws_api-gateway.tf#784) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_base_path_mapping[aws_api_gateway_base_path_mapping.dev]
- .aws_api_gateway_deployment.deployment |(r-aws_api-gateway.tf#679) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_deployment[aws_api_gateway_deployment.deployment]
- .aws_api_gateway_domain_name.api-gateway-domain |(r-aws_api-gateway.tf#775) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_domain_name[aws_api_gateway_domain_name.api-gateway-domain]
- .aws_api_gateway_gateway_response.access_denied |(r-aws_api-gateway.tf#622) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_gateway_response[aws_api_gateway_gateway_response.access_denied]
- .aws_api_gateway_gateway_response.missing_authentication_token |(r-aws_api-gateway.tf#637) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_gateway_response[aws_api_gateway_gateway_response.missing_authentication_token]
- .aws_api_gateway_gateway_response.resource_not_found |(r-aws_api-gateway.tf#651) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_gateway_response[aws_api_gateway_gateway_response.resource_not_found]
- .aws_api_gateway_gateway_response.unauthorized |(r-aws_api-gateway.tf#665) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_gateway_response[aws_api_gateway_gateway_response.unauthorized]
- .aws_api_gateway_integration.api-method-integration-content-proxy |(r-aws_api-gateway.tf#140) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration[aws_api_gateway_integration.api-method-integration-content-proxy]
- .aws_api_gateway_integration.api-method-integration-oauth-proxy |(r-aws_api-gateway.tf#606) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration[aws_api_gateway_integration.api-method-integration-oauth-proxy]
- .aws_api_gateway_integration.api-method-integration-users-proxy |(r-aws_api-gateway.tf#303) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration[aws_api_gateway_integration.api-method-integration-users-proxy]
- .aws_api_gateway_integration.cors_content_integration |(r-aws_api-gateway.tf#129) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration[aws_api_gateway_integration.cors_content_integration]
- .aws_api_gateway_integration.cors_oauth_integration |(r-aws_api-gateway.tf#175) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration[aws_api_gateway_integration.cors_oauth_integration]
- .aws_api_gateway_integration.cors_oauth_validate |(r-aws_api-gateway.tf#344) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration[aws_api_gateway_integration.cors_oauth_validate]
- .aws_api_gateway_integration.cors_oauth_validate_auth |(r-aws_api-gateway.tf#460) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration[aws_api_gateway_integration.cors_oauth_validate_auth]
- .aws_api_gateway_integration.cors_oauth_validate_auth_integration |(r-aws_api-gateway.tf#513) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration[aws_api_gateway_integration.cors_oauth_validate_auth_integration]
- .aws_api_gateway_integration.cors_oauth_validate_integration |(r-aws_api-gateway.tf#395) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration[aws_api_gateway_integration.cors_oauth_validate_integration]
- .aws_api_gateway_integration.cors_users_integration |(r-aws_api-gateway.tf#292) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration[aws_api_gateway_integration.cors_users_integration]
- .aws_api_gateway_integration_response.cors_integration_content_response |(r-aws_api-gateway.tf#108) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration_response[aws_api_gateway_integration_response.cors_integration_content_response]
- .aws_api_gateway_integration_response.cors_integration_oauth_options_response |(r-aws_api-gateway.tf#424) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration_response[aws_api_gateway_integration_response.cors_integration_oauth_options_response]
- .aws_api_gateway_integration_response.cors_integration_oauth_options_response_auth |(r-aws_api-gateway.tf#542) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration_response[aws_api_gateway_integration_response.cors_integration_oauth_options_response_auth]
- .aws_api_gateway_integration_response.cors_integration_oauth_response |(r-aws_api-gateway.tf#157) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration_response[aws_api_gateway_integration_response.cors_integration_oauth_response]
- .aws_api_gateway_integration_response.cors_integration_oauth_validate_auth_response |(r-aws_api-gateway.tf#488) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration_response[aws_api_gateway_integration_response.cors_integration_oauth_validate_auth_response]
- .aws_api_gateway_integration_response.cors_integration_oauth_validate_response |(r-aws_api-gateway.tf#371) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration_response[aws_api_gateway_integration_response.cors_integration_oauth_validate_response]
- .aws_api_gateway_integration_response.cors_integration_users_response |(r-aws_api-gateway.tf#271) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration_response[aws_api_gateway_integration_response.cors_integration_users_response]
- .aws_api_gateway_method.api-method-content-proxy |(r-aws_api-gateway.tf#38) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method[aws_api_gateway_method.api-method-content-proxy]
- .aws_api_gateway_method.api-method-oauth-proxy |(r-aws_api-gateway.tf#566) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method[aws_api_gateway_method.api-method-oauth-proxy]
- .aws_api_gateway_method.api-method-oauth-validate |(r-aws_api-gateway.tf#332) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method[aws_api_gateway_method.api-method-oauth-validate]
- .aws_api_gateway_method.api-method-oauth-validate-auth |(r-aws_api-gateway.tf#448) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method[aws_api_gateway_method.api-method-oauth-validate-auth]
- .aws_api_gateway_method.api-method-user-proxy |(r-aws_api-gateway.tf#202) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method[aws_api_gateway_method.api-method-user-proxy]
- .aws_api_gateway_method.cors_method_content |(r-aws_api-gateway.tf#76) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method[aws_api_gateway_method.cors_method_content]
- .aws_api_gateway_method.cors_method_oauth |(r-aws_api-gateway.tf#577) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method[aws_api_gateway_method.cors_method_oauth]
- .aws_api_gateway_method.cors_method_oauth_validate |(r-aws_api-gateway.tf#384) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method[aws_api_gateway_method.cors_method_oauth_validate]
- .aws_api_gateway_method.cors_method_oauth_validate_auth |(r-aws_api-gateway.tf#502) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method[aws_api_gateway_method.cors_method_oauth_validate_auth]
- .aws_api_gateway_method.cors_method_users |(r-aws_api-gateway.tf#240) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method[aws_api_gateway_method.cors_method_users]
- .aws_api_gateway_method_response.content-service-response-401 |(r-aws_api-gateway.tf#52) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response[aws_api_gateway_method_response.content-service-response-401]
- .aws_api_gateway_method_response.content-service-response-403 |(r-aws_api-gateway.tf#64) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response[aws_api_gateway_method_response.content-service-response-403]
- .aws_api_gateway_method_response.cors_method_content_response |(r-aws_api-gateway.tf#87) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response[aws_api_gateway_method_response.cors_method_content_response]
- .aws_api_gateway_method_response.cors_method_oauth_options_validate |(r-aws_api-gateway.tf#406) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response[aws_api_gateway_method_response.cors_method_oauth_options_validate]
- .aws_api_gateway_method_response.cors_method_oauth_options_validate_auth |(r-aws_api-gateway.tf#524) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response[aws_api_gateway_method_response.cors_method_oauth_options_validate_auth]
- .aws_api_gateway_method_response.cors_method_oauth_response |(r-aws_api-gateway.tf#588) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response[aws_api_gateway_method_response.cors_method_oauth_response]
- .aws_api_gateway_method_response.cors_method_oauth_validate |(r-aws_api-gateway.tf#355) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response[aws_api_gateway_method_response.cors_method_oauth_validate]
- .aws_api_gateway_method_response.cors_method_oauth_validate_auth |(r-aws_api-gateway.tf#471) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response[aws_api_gateway_method_response.cors_method_oauth_validate_auth]
- .aws_api_gateway_method_response.cors_method_users_response |(r-aws_api-gateway.tf#250) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response[aws_api_gateway_method_response.cors_method_users_response]
- .aws_api_gateway_method_response.user-service-response-401 |(r-aws_api-gateway.tf#216) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response[aws_api_gateway_method_response.user-service-response-401]
- .aws_api_gateway_method_response.user-service-response-403 |(r-aws_api-gateway.tf#228) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response[aws_api_gateway_method_response.user-service-response-403]
- .aws_api_gateway_resource.content-proxy |(r-aws_api-gateway.tf#31) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_resource[aws_api_gateway_resource.content-proxy]
- .aws_api_gateway_resource.content-service |(r-aws_api-gateway.tf#22) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_resource[aws_api_gateway_resource.content-service]
- .aws_api_gateway_resource.oauth-keycloak |(r-aws_api-gateway.tf#320) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_resource[aws_api_gateway_resource.oauth-keycloak]
- .aws_api_gateway_resource.oauth-proxy |(r-aws_api-gateway.tf#560) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_resource[aws_api_gateway_resource.oauth-proxy]
- .aws_api_gateway_resource.oauth-validate |(r-aws_api-gateway.tf#326) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_resource[aws_api_gateway_resource.oauth-validate]
- .aws_api_gateway_resource.oauth-validate-auth |(r-aws_api-gateway.tf#442) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_resource[aws_api_gateway_resource.oauth-validate-auth]
- .aws_api_gateway_resource.user-service |(r-aws_api-gateway.tf#188) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_resource[aws_api_gateway_resource.user-service]
- .aws_api_gateway_resource.users-proxy |(r-aws_api-gateway.tf#195) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_resource[aws_api_gateway_resource.users-proxy]
- .aws_api_gateway_rest_api.api |(r-aws_api-gateway.tf#1) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_rest_api[aws_api_gateway_rest_api.api]
## Resources-r-aws_nlb_vpclink.tf
- .aws_api_gateway_vpc_link.api-gateway |(r-aws_nlb_vpclink.tf#39) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_vpc_link[aws_api_gateway_vpc_link.api-gateway]
## Resources-r-aws_kubernetes.tf
- .aws_autoscaling_group.eks_node |(r-aws_kubernetes.tf#67) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/autoscaling_group[aws_autoscaling_group.eks_node]
- .aws_autoscaling_policy.eks_node_policy_down |(r-aws_kubernetes.tf#143) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/autoscaling_policy[aws_autoscaling_policy.eks_node_policy_down]
- .aws_autoscaling_policy.eks_node_policy_up |(r-aws_kubernetes.tf#117) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/autoscaling_policy[aws_autoscaling_policy.eks_node_policy_up]
## Resources-r-aws_api-gateway.tf
- .aws_cloudwatch_event_rule.function_check |(r-aws_api-gateway.tf#815) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_event_rule[aws_cloudwatch_event_rule.function_check]
## Resources-r-aws_lambda_dynamodb_backup.tf
- .aws_cloudwatch_event_rule.schedule-dynamodb-backup |(r-aws_lambda_dynamodb_backup.tf#68) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_event_rule[aws_cloudwatch_event_rule.schedule-dynamodb-backup]
## Resources-r-aws_lambda_es_cleaner.tf
- .aws_cloudwatch_event_rule.schedule-es-cleanup-lambda |(r-aws_lambda_es_cleaner.tf#114) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_event_rule[aws_cloudwatch_event_rule.schedule-es-cleanup-lambda]
## Resources-r-aws_api-gateway.tf
- .aws_cloudwatch_event_target.check_lambda_function |(r-aws_api-gateway.tf#826) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_event_target[aws_cloudwatch_event_target.check_lambda_function]
## Resources-r-aws_lambda_dynamodb_backup.tf
- .aws_cloudwatch_event_target.dynamodb_backup |(r-aws_lambda_dynamodb_backup.tf#74) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_event_target[aws_cloudwatch_event_target.dynamodb_backup]
## Resources-r-aws_lambda_es_cleaner.tf
- .aws_cloudwatch_event_target.es_cleanup |(r-aws_lambda_es_cleaner.tf#120) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_event_target[aws_cloudwatch_event_target.es_cleanup]
- .aws_cloudwatch_log_group.cwlog |(r-aws_lambda_es_cleaner.tf#134) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_log_group[aws_cloudwatch_log_group.cwlog]
## Resources-r-aws_kubernetes.tf
- .aws_cloudwatch_metric_alarm.eks_node_cpu_alarm_down |(r-aws_kubernetes.tf#151) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_metric_alarm[aws_cloudwatch_metric_alarm.eks_node_cpu_alarm_down]
- .aws_cloudwatch_metric_alarm.eks_node_cpu_alarm_up |(r-aws_kubernetes.tf#125) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_metric_alarm[aws_cloudwatch_metric_alarm.eks_node_cpu_alarm_up]
## Resources-r-aws_elasticsearch.tf
- .aws_cloudwatch_metric_alarm.es-disk |(r-aws_elasticsearch.tf#55) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_metric_alarm[aws_cloudwatch_metric_alarm.es-disk]
- .aws_cloudwatch_metric_alarm.es-disk-statistic |(r-aws_elasticsearch.tf#125) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_metric_alarm[aws_cloudwatch_metric_alarm.es-disk-statistic]
## Resources-r-aws_network.tf
- .aws_default_route_table.default |(r-aws_network.tf#43) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/default_route_table[aws_default_route_table.default]
## Resources-r-aws_security.tf
- .aws_default_security_group.default |(r-aws_security.tf#2) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/default_security_group[aws_default_security_group.default]
## Resources-r-aws_dynamodb.tf
- .aws_dynamodb_table.applet |(r-aws_dynamodb.tf#20) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.applet]
- .aws_dynamodb_table.bs_iccid_info |(r-aws_dynamodb.tf#254) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.bs_iccid_info]
- .aws_dynamodb_table.campaign |(r-aws_dynamodb.tf#54) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.campaign]
- .aws_dynamodb_table.campaign_execution |(r-aws_dynamodb.tf#101) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.campaign_execution]
- .aws_dynamodb_table.co_campaign_execution |(r-aws_dynamodb.tf#837) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.co_campaign_execution]
- .aws_dynamodb_table.co_script_execution |(r-aws_dynamodb.tf#857) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.co_script_execution]
- .aws_dynamodb_table.co_vendor |(r-aws_dynamodb.tf#1) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.co_vendor]
- .aws_dynamodb_table.cs_api_key |(r-aws_dynamodb.tf#911) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.cs_api_key]
- .aws_dynamodb_table.cs_campaign_execution |(r-aws_dynamodb.tf#951) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.cs_campaign_execution]
- .aws_dynamodb_table.cs_ce_command_execution |(r-aws_dynamodb.tf#1134) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.cs_ce_command_execution]
- .aws_dynamodb_table.cs_grouped_commands |(r-aws_dynamodb.tf#1179) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.cs_grouped_commands]
- .aws_dynamodb_table.cs_script_execution |(r-aws_dynamodb.tf#986) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.cs_script_execution]
- .aws_dynamodb_table.cs_vendor_permissions |(r-aws_dynamodb.tf#650) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.cs_vendor_permissions]
- .aws_dynamodb_table.custom_commands |(r-aws_dynamodb.tf#1216) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.custom_commands]
- .aws_dynamodb_table.device_command |(r-aws_dynamodb.tf#148) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.device_command]
- .aws_dynamodb_table.device_config_links |(r-aws_dynamodb.tf#478) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.device_config_links]
- .aws_dynamodb_table.device_info |(r-aws_dynamodb.tf#201) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.device_info]
- .aws_dynamodb_table.device_notifications |(r-aws_dynamodb.tf#328) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.device_notifications]
- .aws_dynamodb_table.dg_api_key |(r-aws_dynamodb.tf#931) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.dg_api_key]
- .aws_dynamodb_table.dg_vendor |(r-aws_dynamodb.tf#743) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.dg_vendor]
- .aws_dynamodb_table.es_user_info |(r-aws_dynamodb.tf#1074) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.es_user_info]
- .aws_dynamodb_table.es_vendor_info |(r-aws_dynamodb.tf#1094) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.es_vendor_info]
- .aws_dynamodb_table.gp_applet |(r-aws_dynamodb.tf#274) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.gp_applet]
- .aws_dynamodb_table.gp_command_preparation |(r-aws_dynamodb.tf#1159) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.gp_command_preparation]
- .aws_dynamodb_table.group |(r-aws_dynamodb.tf#294) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.group]
- .aws_dynamodb_table.iccid |(r-aws_dynamodb.tf#1256) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.iccid]
- .aws_dynamodb_table.identities |(r-aws_dynamodb.tf#1324) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.identities]
- .aws_dynamodb_table.kcss_command_preparation |(r-aws_dynamodb.tf#1114) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.kcss_command_preparation]
- .aws_dynamodb_table.ks_iccid_info |(r-aws_dynamodb.tf#1236) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.ks_iccid_info]
- .aws_dynamodb_table.pa_applet_commands |(r-aws_dynamodb.tf#537) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.pa_applet_commands]
- .aws_dynamodb_table.proxy_applet_session_info |(r-aws_dynamodb.tf#127) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.proxy_applet_session_info]
- .aws_dynamodb_table.relation_profile |(r-aws_dynamodb.tf#367) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.relation_profile]
- .aws_dynamodb_table.role |(r-aws_dynamodb.tf#400) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.role]
- .aws_dynamodb_table.scheduled_event |(r-aws_dynamodb.tf#439) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.scheduled_event]
- .aws_dynamodb_table.script |(r-aws_dynamodb.tf#576) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.script]
- .aws_dynamodb_table.script_execution |(r-aws_dynamodb.tf#609) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.script_execution]
- .aws_dynamodb_table.script_template |(r-aws_dynamodb.tf#498) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.script_template]
- .aws_dynamodb_table.se_device_info |(r-aws_dynamodb.tf#221) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.se_device_info]
- .aws_dynamodb_table.supported_commands |(r-aws_dynamodb.tf#630) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.supported_commands]
- .aws_dynamodb_table.uicc |(r-aws_dynamodb.tf#670) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.uicc]
- .aws_dynamodb_table.uicc_group |(r-aws_dynamodb.tf#710) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.uicc_group]
- .aws_dynamodb_table.us_api_key |(r-aws_dynamodb.tf#891) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.us_api_key]
- .aws_dynamodb_table.us_supported_ca |(r-aws_dynamodb.tf#168) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.us_supported_ca]
- .aws_dynamodb_table.user |(r-aws_dynamodb.tf#763) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.user]
- .aws_dynamodb_table.vendor |(r-aws_dynamodb.tf#1028) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table[aws_dynamodb_table.vendor]
## Resources-r-aws_efs.tf
- .aws_efs_file_system.efs_key_service |(r-aws_efs.tf#20) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/efs_file_system[aws_efs_file_system.efs_key_service]
- .aws_efs_file_system_policy.policy |(r-aws_efs.tf#34) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/efs_file_system_policy[aws_efs_file_system_policy.policy]
- .aws_efs_mount_target.efs_key_service |(r-aws_efs.tf#27) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/efs_mount_target[aws_efs_mount_target.efs_key_service]
## Resources-r-aws_network.tf
- .aws_eip.eip_1 |(r-aws_network.tf#25) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip[aws_eip.eip_1]
- .aws_eip.eip_2 |(r-aws_network.tf#32) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip[aws_eip.eip_2]
- .aws_eip.eip_3_proxy_applet |(r-aws_network.tf#160) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip[aws_eip.eip_3_proxy_applet]
- .aws_eip_association.infrastructure_bastion_eip_association |(r-aws_network.tf#37) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip_association[aws_eip_association.infrastructure_bastion_eip_association]
## Resources-r-aws_kubernetes.tf
- .aws_eks_cluster.cluster |(r-aws_kubernetes.tf#11) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eks_cluster[aws_eks_cluster.cluster]
## Resources-r-aws_elasticsearch.tf
- .aws_elasticsearch_domain.es_apps_logs_storage |(r-aws_elasticsearch.tf#1) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/elasticsearch_domain[aws_elasticsearch_domain.es_apps_logs_storage]
- .aws_elasticsearch_domain.es_apps_logs_storage_statistic |(r-aws_elasticsearch.tf#71) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/elasticsearch_domain[aws_elasticsearch_domain.es_apps_logs_storage_statistic]
## Resources-r-aws_iam_apps.tf
- .aws_iam_access_key.backup_user |(r-aws_iam_apps.tf#1154) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_access_key[aws_iam_access_key.backup_user]
## Resources-r-aws_iam.tf
- .aws_iam_access_key.mail_sender_user |(r-aws_iam.tf#302) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_access_key[aws_iam_access_key.mail_sender_user]
- .aws_iam_instance_profile.eks-instance |(r-aws_iam.tf#76) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_instance_profile[aws_iam_instance_profile.eks-instance]
## Resources-r-aws_kubernetes.tf
- .aws_iam_openid_connect_provider.this |(r-aws_kubernetes.tf#197) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_openid_connect_provider[aws_iam_openid_connect_provider.this]
## Resources-r-aws_iam_apps.tf
- .aws_iam_policy.backup_user |(r-aws_iam_apps.tf#1159) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.backup_user]
## Resources-r-aws_iam.tf
- .aws_iam_policy.eks-albingress |(r-aws_iam.tf#138) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.eks-albingress]
- .aws_iam_policy.eks-albingress-dns |(r-aws_iam.tf#257) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.eks-albingress-dns]
## Resources-r-aws_iam_apps.tf
- .aws_iam_policy.eks-cluster-autoscaler |(r-aws_iam_apps.tf#1111) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.eks-cluster-autoscaler]
## Resources-r-aws_iam.tf
- .aws_iam_policy.grafana-datasource-cloudwatch |(r-aws_iam.tf#81) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.grafana-datasource-cloudwatch]
## Resources-r-aws_lambda_iam_role.tf
- .aws_iam_policy.kms_full_access |(r-aws_lambda_iam_role.tf#25) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.kms_full_access]
## Resources-r-aws_lambda_es_cleaner.tf
- .aws_iam_policy.lambda_es_access |(r-aws_lambda_es_cleaner.tf#68) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.lambda_es_access]
## Resources-r-aws_iam_prometheus.tf
- .aws_iam_policy.prometheus |(r-aws_iam_prometheus.tf#7) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.prometheus]
## Resources-r-aws_iam.tf
- .aws_iam_policy.ses |(r-aws_iam.tf#311) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.ses]
## Resources-r-aws_iam_apps.tf
- .aws_iam_policy.vsts-bootstrap-service |(r-aws_iam_apps.tf#831) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.vsts-bootstrap-service]
- .aws_iam_policy.vsts-campaign-orchestrator |(r-aws_iam_apps.tf#7) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.vsts-campaign-orchestrator]
- .aws_iam_policy.vsts-ci-service |(r-aws_iam_apps.tf#71) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.vsts-ci-service]
- .aws_iam_policy.vsts-content-service |(r-aws_iam_apps.tf#132) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.vsts-content-service]
- .aws_iam_policy.vsts-crypto-service |(r-aws_iam_apps.tf#226) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.vsts-crypto-service]
- .aws_iam_policy.vsts-device-gateway |(r-aws_iam_apps.tf#637) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.vsts-device-gateway]
- .aws_iam_policy.vsts-dim-service |(r-aws_iam_apps.tf#530) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.vsts-dim-service]
- .aws_iam_policy.vsts-event-scheduler |(r-aws_iam_apps.tf#287) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.vsts-event-scheduler]
- .aws_iam_policy.vsts-gp-service |(r-aws_iam_apps.tf#764) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.vsts-gp-service]
- .aws_iam_policy.vsts-kcss-service |(r-aws_iam_apps.tf#342) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.vsts-kcss-service]
- .aws_iam_policy.vsts-key-service |(r-aws_iam_apps.tf#580) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.vsts-key-service]
- .aws_iam_policy.vsts-notification-service |(r-aws_iam_apps.tf#924) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.vsts-notification-service]
- .aws_iam_policy.vsts-proxy-applet-service |(r-aws_iam_apps.tf#1021) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.vsts-proxy-applet-service]
- .aws_iam_policy.vsts-script-executor |(r-aws_iam_apps.tf#403) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.vsts-script-executor]
- .aws_iam_policy.vsts-sms-service |(r-aws_iam_apps.tf#1077) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.vsts-sms-service]
- .aws_iam_policy.vsts-statistic-service |(r-aws_iam_apps.tf#977) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.vsts-statistic-service]
- .aws_iam_policy.vsts-user-service |(r-aws_iam_apps.tf#467) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy[aws_iam_policy.vsts-user-service]
## Resources-r-aws_iam.tf
- .aws_iam_policy_attachment.attach_eks-albingress |(r-aws_iam.tf#251) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy_attachment[aws_iam_policy_attachment.attach_eks-albingress]
- .aws_iam_policy_attachment.attach_eks-albingress-dns |(r-aws_iam.tf#289) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy_attachment[aws_iam_policy_attachment.attach_eks-albingress-dns]
## Resources-r-aws_iotcore.tf
- .aws_iam_role.device_onboard |(r-aws_iotcore.tf#175) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.device_onboard]
## Resources-r-aws_lambda_dynamodb_backup.tf
- .aws_iam_role.dynamo_db_backup |(r-aws_lambda_dynamodb_backup.tf#2) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.dynamo_db_backup]
## Resources-r-aws_iam.tf
- .aws_iam_role.eks |(r-aws_iam.tf#1) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.eks]
## Resources-r-aws_iam_apps.tf
- .aws_iam_role.eks-cluster-autoscaler |(r-aws_iam_apps.tf#1137) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.eks-cluster-autoscaler]
## Resources-r-aws_iam.tf
- .aws_iam_role.eks-instance |(r-aws_iam.tf#34) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.eks-instance]
## Resources-r-aws_api-gateway.tf
- .aws_iam_role.invocation_role |(r-aws_api-gateway.tf#859) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.invocation_role]
- .aws_iam_role.lambda-api-gateway |(r-aws_api-gateway.tf#899) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.lambda-api-gateway]
## Resources-r-aws_iam_apps.tf
- .aws_iam_role.openldap_dlm_lifecycle_role |(r-aws_iam_apps.tf#1203) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.openldap_dlm_lifecycle_role]
## Resources-r-aws_iam_prometheus.tf
- .aws_iam_role.prometheus |(r-aws_iam_prometheus.tf#2) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.prometheus]
## Resources-r-aws_iotcore.tf
- .aws_iam_role.se_events |(r-aws_iotcore.tf#353) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.se_events]
- .aws_iam_role.se_status |(r-aws_iotcore.tf#264) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.se_status]
## Resources-r-aws_iam_apps.tf
- .aws_iam_role.vsts-bootstrap-service |(r-aws_iam_apps.tf#826) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.vsts-bootstrap-service]
- .aws_iam_role.vsts-campaign-orchestrator |(r-aws_iam_apps.tf#2) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.vsts-campaign-orchestrator]
- .aws_iam_role.vsts-ci-service |(r-aws_iam_apps.tf#66) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.vsts-ci-service]
- .aws_iam_role.vsts-content-service |(r-aws_iam_apps.tf#127) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.vsts-content-service]
- .aws_iam_role.vsts-crypto-service |(r-aws_iam_apps.tf#221) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.vsts-crypto-service]
- .aws_iam_role.vsts-device-gateway |(r-aws_iam_apps.tf#631) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.vsts-device-gateway]
- .aws_iam_role.vsts-dim-service |(r-aws_iam_apps.tf#525) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.vsts-dim-service]
- .aws_iam_role.vsts-event-scheduler |(r-aws_iam_apps.tf#282) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.vsts-event-scheduler]
- .aws_iam_role.vsts-gp-service |(r-aws_iam_apps.tf#759) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.vsts-gp-service]
- .aws_iam_role.vsts-kcss-service |(r-aws_iam_apps.tf#337) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.vsts-kcss-service]
- .aws_iam_role.vsts-key-service |(r-aws_iam_apps.tf#575) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.vsts-key-service]
- .aws_iam_role.vsts-notification-service |(r-aws_iam_apps.tf#919) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.vsts-notification-service]
- .aws_iam_role.vsts-proxy-applet-service |(r-aws_iam_apps.tf#1016) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.vsts-proxy-applet-service]
- .aws_iam_role.vsts-script-executor |(r-aws_iam_apps.tf#398) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.vsts-script-executor]
- .aws_iam_role.vsts-sms-service |(r-aws_iam_apps.tf#1072) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.vsts-sms-service]
- .aws_iam_role.vsts-statistic-service |(r-aws_iam_apps.tf#972) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.vsts-statistic-service]
- .aws_iam_role.vsts-user-service |(r-aws_iam_apps.tf#462) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.vsts-user-service]
## Resources-r-aws_lambda_iam_role.tf
- .aws_iam_role.vsts_lambda_db_campaign_execution |(r-aws_lambda_iam_role.tf#2) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.vsts_lambda_db_campaign_execution]
## Resources-r-aws_lambda_es_cleaner.tf
- .aws_iam_role.vsts_lambda_es_cleanup |(r-aws_lambda_es_cleaner.tf#45) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role[aws_iam_role.vsts_lambda_es_cleanup]
## Resources-r-aws_iotcore.tf
- .aws_iam_role_policy.device_onboard |(r-aws_iotcore.tf#194) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy[aws_iam_role_policy.device_onboard]
## Resources-r-aws_api-gateway.tf
- .aws_iam_role_policy.invocation_policy |(r-aws_api-gateway.tf#881) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy[aws_iam_role_policy.invocation_policy]
## Resources-r-aws_iam_apps.tf
- .aws_iam_role_policy.openldap_dlm_lifecycle_role_policy |(r-aws_iam_apps.tf#1224) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy[aws_iam_role_policy.openldap_dlm_lifecycle_role_policy]
## Resources-r-aws_iotcore.tf
- .aws_iam_role_policy.se_events |(r-aws_iotcore.tf#372) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy[aws_iam_role_policy.se_events]
- .aws_iam_role_policy.se_status |(r-aws_iotcore.tf#283) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy[aws_iam_role_policy.se_status]
## Resources-r-aws_lambda_iam_role.tf
- .aws_iam_role_policy_attachment.AmazonDynamoDBFullAccess |(r-aws_lambda_iam_role.tf#43) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.AmazonDynamoDBFullAccess]
## Resources-r-aws_lambda_dynamodb_backup.tf
- .aws_iam_role_policy_attachment.AmazonDynamoDBFullAccess_dynamod_backup |(r-aws_lambda_dynamodb_backup.tf#25) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.AmazonDynamoDBFullAccess_dynamod_backup]
## Resources-r-aws_lambda_iam_role.tf
- .aws_iam_role_policy_attachment.AmazonSNSFullAccess |(r-aws_lambda_iam_role.tf#48) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.AmazonSNSFullAccess]
- .aws_iam_role_policy_attachment.CloudWatchFullAccess |(r-aws_lambda_iam_role.tf#53) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.CloudWatchFullAccess]
## Resources-r-aws_api-gateway.tf
- .aws_iam_role_policy_attachment.CloudWatchFullAccess-lambda-api-gateway |(r-aws_api-gateway.tf#919) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.CloudWatchFullAccess-lambda-api-gateway]
## Resources-r-aws_lambda_dynamodb_backup.tf
- .aws_iam_role_policy_attachment.CloudWatchFullAccess_dynamod_backup |(r-aws_lambda_dynamodb_backup.tf#30) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.CloudWatchFullAccess_dynamod_backup]
## Resources-r-aws_lambda_iam_role.tf
- .aws_iam_role_policy_attachment.KMSFullAccess |(r-aws_lambda_iam_role.tf#58) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.KMSFullAccess]
## Resources-r-aws_lambda_dynamodb_backup.tf
- .aws_iam_role_policy_attachment.KMSFullAccess_dynamod_backup |(r-aws_lambda_dynamodb_backup.tf#35) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.KMSFullAccess_dynamod_backup]
## Resources-r-aws_iam.tf
- .aws_iam_role_policy_attachment.eks-AmazonEKSClusterPolicy |(r-aws_iam.tf#23) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.eks-AmazonEKSClusterPolicy]
- .aws_iam_role_policy_attachment.eks-AmazonEKSServicePolicy |(r-aws_iam.tf#28) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.eks-AmazonEKSServicePolicy]
## Resources-r-aws_iam_apps.tf
- .aws_iam_role_policy_attachment.eks-cluster-autoscaler |(r-aws_iam_apps.tf#1142) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.eks-cluster-autoscaler]
## Resources-r-aws_iam.tf
- .aws_iam_role_policy_attachment.eks-instance-AmazonCloudwatchGrafana |(r-aws_iam.tf#71) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.eks-instance-AmazonCloudwatchGrafana]
- .aws_iam_role_policy_attachment.eks-instance-AmazonEC2ContainerRegistryReadOnly |(r-aws_iam.tf#66) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.eks-instance-AmazonEC2ContainerRegistryReadOnly]
- .aws_iam_role_policy_attachment.eks-instance-AmazonEKSWorkerNodePolicy |(r-aws_iam.tf#56) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.eks-instance-AmazonEKSWorkerNodePolicy]
- .aws_iam_role_policy_attachment.eks-instance-AmazonEKS_CNI_Policy |(r-aws_iam.tf#61) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.eks-instance-AmazonEKS_CNI_Policy]
## Resources-r-aws_lambda_es_cleaner.tf
- .aws_iam_role_policy_attachment.lambda-es-permission |(r-aws_lambda_es_cleaner.tf#109) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.lambda-es-permission]
## Resources-r-aws_iam_prometheus.tf
- .aws_iam_role_policy_attachment.prometheus |(r-aws_iam_prometheus.tf#35) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.prometheus]
## Resources-r-aws_iam_apps.tf
- .aws_iam_role_policy_attachment.vsts-bootstrap-service |(r-aws_iam_apps.tf#913) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.vsts-bootstrap-service]
- .aws_iam_role_policy_attachment.vsts-campaign-orchestrator |(r-aws_iam_apps.tf#60) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.vsts-campaign-orchestrator]
- .aws_iam_role_policy_attachment.vsts-ci-service |(r-aws_iam_apps.tf#121) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.vsts-ci-service]
- .aws_iam_role_policy_attachment.vsts-content-service |(r-aws_iam_apps.tf#215) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.vsts-content-service]
- .aws_iam_role_policy_attachment.vsts-crypto-service |(r-aws_iam_apps.tf#276) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.vsts-crypto-service]
- .aws_iam_role_policy_attachment.vsts-device-gateway |(r-aws_iam_apps.tf#753) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.vsts-device-gateway]
- .aws_iam_role_policy_attachment.vsts-dim-service |(r-aws_iam_apps.tf#569) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.vsts-dim-service]
- .aws_iam_role_policy_attachment.vsts-event-scheduler |(r-aws_iam_apps.tf#331) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.vsts-event-scheduler]
- .aws_iam_role_policy_attachment.vsts-gp-service |(r-aws_iam_apps.tf#820) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.vsts-gp-service]
- .aws_iam_role_policy_attachment.vsts-kcss-service |(r-aws_iam_apps.tf#392) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.vsts-kcss-service]
- .aws_iam_role_policy_attachment.vsts-key-service |(r-aws_iam_apps.tf#625) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.vsts-key-service]
- .aws_iam_role_policy_attachment.vsts-notification-service |(r-aws_iam_apps.tf#966) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.vsts-notification-service]
- .aws_iam_role_policy_attachment.vsts-proxy-applet-service |(r-aws_iam_apps.tf#1066) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.vsts-proxy-applet-service]
- .aws_iam_role_policy_attachment.vsts-script-executor |(r-aws_iam_apps.tf#456) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.vsts-script-executor]
- .aws_iam_role_policy_attachment.vsts-sms-service |(r-aws_iam_apps.tf#1105) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.vsts-sms-service]
- .aws_iam_role_policy_attachment.vsts-statistic-service |(r-aws_iam_apps.tf#1010) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.vsts-statistic-service]
- .aws_iam_role_policy_attachment.vsts-user-service |(r-aws_iam_apps.tf#519) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment[aws_iam_role_policy_attachment.vsts-user-service]
- .aws_iam_user.backup_user |(r-aws_iam_apps.tf#1148) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_user[aws_iam_user.backup_user]
## Resources-r-aws_iam.tf
- .aws_iam_user.mail_sender_user |(r-aws_iam.tf#296) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_user[aws_iam_user.mail_sender_user]
## Resources-r-aws_iam_apps.tf
- .aws_iam_user_policy_attachment.backup_user |(r-aws_iam_apps.tf#1197) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_user_policy_attachment[aws_iam_user_policy_attachment.backup_user]
## Resources-r-aws_iam.tf
- .aws_iam_user_policy_attachment.ses |(r-aws_iam.tf#306) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_user_policy_attachment[aws_iam_user_policy_attachment.ses]
## Resources-r-aws_ec2.tf
- .aws_instance.bastion |(r-aws_ec2.tf#1) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/instance[aws_instance.bastion]
## Resources-r-aws_openldap.tf
- .aws_instance.openldap |(r-aws_openldap.tf#8) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/instance[aws_instance.openldap]
## Resources-r-aws_network.tf
- .aws_internet_gateway.igw_1 |(r-aws_network.tf#11) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/internet_gateway[aws_internet_gateway.igw_1]
## Resources-r-aws_iotcore.tf
- .aws_iot_certificate.cert_thing_backend_client |(r-aws_iotcore.tf#31) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_certificate[aws_iot_certificate.cert_thing_backend_client]
- .aws_iot_certificate.cert_thing_bootstrap |(r-aws_iotcore.tf#27) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_certificate[aws_iot_certificate.cert_thing_bootstrap]
- .aws_iot_policy.policy_thing |(r-aws_iotcore.tf#74) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_policy[aws_iot_policy.policy_thing]
- .aws_iot_policy.policy_thing_backend_client |(r-aws_iotcore.tf#55) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_policy[aws_iot_policy.policy_thing_backend_client]
- .aws_iot_policy.policy_thing_bootstrap |(r-aws_iotcore.tf#36) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_policy[aws_iot_policy.policy_thing_bootstrap]
- .aws_iot_policy_attachment.policy_thing_attachment |(r-aws_iotcore.tf#128) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_policy_attachment[aws_iot_policy_attachment.policy_thing_attachment]
- .aws_iot_policy_attachment.policy_thing_backend_client_attachment |(r-aws_iotcore.tf#138) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_policy_attachment[aws_iot_policy_attachment.policy_thing_backend_client_attachment]
- .aws_iot_policy_attachment.policy_thing_bootstrap_attachment |(r-aws_iotcore.tf#123) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_policy_attachment[aws_iot_policy_attachment.policy_thing_bootstrap_attachment]
- .aws_iot_thing.thing_backend_client |(r-aws_iotcore.tf#16) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_thing[aws_iot_thing.thing_backend_client]
- .aws_iot_thing.thing_bootstrap |(r-aws_iotcore.tf#7) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_thing[aws_iot_thing.thing_bootstrap]
- .aws_iot_thing_principal_attachment.principal_thing_backend_client_attachment |(r-aws_iotcore.tf#143) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_thing_principal_attachment[aws_iot_thing_principal_attachment.principal_thing_backend_client_attachment]
- .aws_iot_thing_principal_attachment.principal_thing_bootstrap_attachment |(r-aws_iotcore.tf#133) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_thing_principal_attachment[aws_iot_thing_principal_attachment.principal_thing_bootstrap_attachment]
- .aws_iot_thing_type.type1 |(r-aws_iotcore.tf#2) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_thing_type[aws_iot_thing_type.type1]
- .aws_iot_topic_rule.device_onboard |(r-aws_iotcore.tf#149) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_topic_rule[aws_iot_topic_rule.device_onboard]
- .aws_iot_topic_rule.se_events |(r-aws_iotcore.tf#327) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_topic_rule[aws_iot_topic_rule.se_events]
- .aws_iot_topic_rule.se_status |(r-aws_iotcore.tf#238) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_topic_rule[aws_iot_topic_rule.se_status]
## Resources-r-aws_kubernetes.tf
- .aws_key_pair.eks-node |(r-aws_kubernetes.tf#46) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/key_pair[aws_key_pair.eks-node]
## Resources-r-aws_kms.tf
- .aws_kms_alias.common_key |(r-aws_kms.tf#120) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/kms_alias[aws_kms_alias.common_key]
- .aws_kms_key.common_key |(r-aws_kms.tf#2) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/kms_key[aws_kms_key.common_key]
## Resources-r-aws_lambda_iam_role.tf
- .aws_lambda_event_source_mapping.lambda-db-campaign-execution-trigger |(r-aws_lambda_iam_role.tf#87) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_event_source_mapping[aws_lambda_event_source_mapping.lambda-db-campaign-execution-trigger]
## Resources-r-aws_api-gateway.tf
- .aws_lambda_function.authorizer |(r-aws_api-gateway.tf#795) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_function[aws_lambda_function.authorizer]
## Resources-r-aws_lambda_iam_role.tf
- .aws_lambda_function.db-campaign-execution |(r-aws_lambda_iam_role.tf#64) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_function[aws_lambda_function.db-campaign-execution]
## Resources-r-aws_lambda_dynamodb_backup.tf
- .aws_lambda_function.dynamodb-backup |(r-aws_lambda_dynamodb_backup.tf#48) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_function[aws_lambda_function.dynamodb-backup]
## Resources-r-aws_lambda_es_cleaner.tf
- .aws_lambda_function.vsts_es_cleanup |(r-aws_lambda_es_cleaner.tf#16) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_function[aws_lambda_function.vsts_es_cleanup]
- .aws_lambda_permission.allow_cloudwatch |(r-aws_lambda_es_cleaner.tf#126) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_permission[aws_lambda_permission.allow_cloudwatch]
## Resources-r-aws_lambda_dynamodb_backup.tf
- .aws_lambda_permission.allow_cloudwatch_dynamod_backup |(r-aws_lambda_dynamodb_backup.tf#80) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_permission[aws_lambda_permission.allow_cloudwatch_dynamod_backup]
## Resources-r-aws_api-gateway.tf
- .aws_lambda_permission.allow_cloudwatch_to_call_function |(r-aws_api-gateway.tf#838) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_permission[aws_lambda_permission.allow_cloudwatch_to_call_function]
## Resources-r-aws_kubernetes.tf
- .aws_launch_configuration.eks_node |(r-aws_kubernetes.tf#51) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/launch_configuration[aws_launch_configuration.eks_node]
## Resources-r-aws_nlb_vpclink.tf
- .aws_lb.load_balancer |(r-aws_nlb_vpclink.tf#1) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb[aws_lb.load_balancer]
## Resources-r-aws_nlb_proxy_applet.tf
- .aws_lb.load_balancer_proxy_applet |(r-aws_nlb_proxy_applet.tf#1) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb[aws_lb.load_balancer_proxy_applet]
## Resources-r-aws_openldap.tf
- .aws_lb.openldap |(r-aws_openldap.tf#36) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb[aws_lb.openldap]
## Resources-r-aws_nlb_wireguard.tf
- .aws_lb.wireguard_lb |(r-aws_nlb_wireguard.tf#1) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb[aws_lb.wireguard_lb]
## Resources-r-aws_nlb_vpclink.tf
- .aws_lb_listener.listener |(r-aws_nlb_vpclink.tf#9) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_listener[aws_lb_listener.listener]
## Resources-r-aws_nlb_proxy_applet.tf
- .aws_lb_listener.listener-proxy-applet |(r-aws_nlb_proxy_applet.tf#13) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_listener[aws_lb_listener.listener-proxy-applet]
## Resources-r-aws_openldap.tf
- .aws_lb_listener.openldap_port443 |(r-aws_openldap.tf#70) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_listener[aws_lb_listener.openldap_port443]
- .aws_lb_listener.openldap_port80 |(r-aws_openldap.tf#84) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_listener[aws_lb_listener.openldap_port80]
## Resources-r-aws_nlb_wireguard.tf
- .aws_lb_listener.wireguard_listener |(r-aws_nlb_wireguard.tf#9) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_listener[aws_lb_listener.wireguard_listener]
## Resources-r-aws_nlb_vpclink.tf
- .aws_lb_target_group.nlb-tg |(r-aws_nlb_vpclink.tf#21) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_target_group[aws_lb_target_group.nlb-tg]
## Resources-r-aws_nlb_proxy_applet.tf
- .aws_lb_target_group.nlb-tg-proxy-applet |(r-aws_nlb_proxy_applet.tf#25) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_target_group[aws_lb_target_group.nlb-tg-proxy-applet]
## Resources-r-aws_openldap.tf
- .aws_lb_target_group.openldap |(r-aws_openldap.tf#47) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_target_group[aws_lb_target_group.openldap]
## Resources-r-aws_nlb_wireguard.tf
- .aws_lb_target_group.wireguard-tg |(r-aws_nlb_wireguard.tf#20) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_target_group[aws_lb_target_group.wireguard-tg]
## Resources-r-aws_openldap.tf
- .aws_lb_target_group_attachment.openldap |(r-aws_openldap.tf#101) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_target_group_attachment[aws_lb_target_group_attachment.openldap]
## Resources-r-aws_network.tf
- .aws_nat_gateway.natgw_1 |(r-aws_network.tf#17) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/nat_gateway[aws_nat_gateway.natgw_1]
## Resources-r-aws_api-gateway.tf
- .aws_route53_record.api-gateway |(r-aws_api-gateway.tf#719) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route53_record[aws_route53_record.api-gateway]
- .aws_route53_record.api_gateway_cert_validation |(r-aws_api-gateway.tf#736) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route53_record[aws_route53_record.api_gateway_cert_validation]
## Resources-r-aws_openldap.tf
- .aws_route53_record.openldap |(r-aws_openldap.tf#108) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route53_record[aws_route53_record.openldap]
- .aws_route53_record.openldap_cert_validation |(r-aws_openldap.tf#136) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route53_record[aws_route53_record.openldap_cert_validation]
## Resources-r-aws_s3.tf
- .aws_route53_record.storage-documentation |(r-aws_s3.tf#94) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route53_record[aws_route53_record.storage-documentation]
## Resources-r-aws_route53.tf
- .aws_route53_record.wildcard_cert_validation |(r-aws_route53.tf#20) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route53_record[aws_route53_record.wildcard_cert_validation]
- .aws_route53_record.wireguard |(r-aws_route53.tf#2) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route53_record[aws_route53_record.wireguard]
## Resources-r-aws_network.tf
- .aws_route_table.private |(r-aws_network.tf#60) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table[aws_route_table.private]
- .aws_route_table.public |(r-aws_network.tf#49) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table[aws_route_table.public]
- .aws_route_table_association.private_1 |(r-aws_network.tf#127) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association[aws_route_table_association.private_1]
- .aws_route_table_association.private_2 |(r-aws_network.tf#141) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association[aws_route_table_association.private_2]
- .aws_route_table_association.private_3 |(r-aws_network.tf#155) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association[aws_route_table_association.private_3]
- .aws_route_table_association.public_1 |(r-aws_network.tf#85) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association[aws_route_table_association.public_1]
- .aws_route_table_association.public_2 |(r-aws_network.tf#99) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association[aws_route_table_association.public_2]
- .aws_route_table_association.public_3 |(r-aws_network.tf#113) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association[aws_route_table_association.public_3]
## Resources-r-aws_s3.tf
- .aws_s3_bucket.backup_bucket |(r-aws_s3.tf#109) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket[aws_s3_bucket.backup_bucket]
- .aws_s3_bucket.ca-certificates |(r-aws_s3.tf#10) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket[aws_s3_bucket.ca-certificates]
- .aws_s3_bucket.campaign-execution |(r-aws_s3.tf#17) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket[aws_s3_bucket.campaign-execution]
- .aws_s3_bucket.device-configuration |(r-aws_s3.tf#2) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket[aws_s3_bucket.device-configuration]
- .aws_s3_bucket.dim-certificate |(r-aws_s3.tf#25) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket[aws_s3_bucket.dim-certificate]
- .aws_s3_bucket.prometheus |(r-aws_s3.tf#33) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket[aws_s3_bucket.prometheus]
- .aws_s3_bucket.static-site-documentation |(r-aws_s3.tf#42) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket[aws_s3_bucket.static-site-documentation]
- .aws_s3_bucket_object.openldap_backup_folder |(r-aws_s3.tf#127) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket_object[aws_s3_bucket_object.openldap_backup_folder]
- .aws_s3_bucket_policy.static-site-documentation_policy |(r-aws_s3.tf#57) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket_policy[aws_s3_bucket_policy.static-site-documentation_policy]
## Resources-r-aws_efs.tf
- .aws_security_group.efs-sg |(r-aws_efs.tf#1) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group[aws_security_group.efs-sg]
## Resources-r-aws_security.tf
- .aws_security_group.eks |(r-aws_security.tf#107) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group[aws_security_group.eks]
- .aws_security_group.eks-node |(r-aws_security.tf#138) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group[aws_security_group.eks-node]
- .aws_security_group.eks-node-test |(r-aws_security.tf#231) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group[aws_security_group.eks-node-test]
## Resources-r-aws_lambda_es_cleaner.tf
- .aws_security_group.es_cleanup |(r-aws_lambda_es_cleaner.tf#2) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group[aws_security_group.es_cleanup]
## Resources-r-aws_openldap.tf
- .aws_security_group.openldap_alb |(r-aws_openldap.tf#204) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group[aws_security_group.openldap_alb]
- .aws_security_group.openldap_ec2 |(r-aws_openldap.tf#161) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group[aws_security_group.openldap_ec2]
## Resources-r-aws_security.tf
- .aws_security_group.sg_bastion |(r-aws_security.tf#189) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group[aws_security_group.sg_bastion]
- .aws_security_group.sg_common |(r-aws_security.tf#21) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group[aws_security_group.sg_common]
- .aws_security_group.sg_es |(r-aws_security.tf#78) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group[aws_security_group.sg_es]
- .aws_security_group_rule.http |(r-aws_security.tf#248) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group_rule[aws_security_group_rule.http]
- .aws_security_group_rule.ingress-eks |(r-aws_security.tf#179) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group_rule[aws_security_group_rule.ingress-eks]
- .aws_security_group_rule.ingress-node-https |(r-aws_security.tf#129) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group_rule[aws_security_group_rule.ingress-node-https]
- .aws_security_group_rule.ingress-self |(r-aws_security.tf#170) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group_rule[aws_security_group_rule.ingress-self]
- .aws_security_group_rule.ingress-workstation-https |(r-aws_security.tf#120) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group_rule[aws_security_group_rule.ingress-workstation-https]
## Resources-r-aws_ses.tf
- .aws_ses_email_identity.mail_sender_user |(r-aws_ses.tf#1) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ses_email_identity[aws_ses_email_identity.mail_sender_user]
## Resources-r-aws_sns.tf
- .aws_sns_platform_application.fcm_application |(r-aws_sns.tf#641) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_platform_application[aws_sns_platform_application.fcm_application]
- .aws_sns_topic.applet_events |(r-aws_sns.tf#37) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.applet_events]
- .aws_sns_topic.bootstrap_events |(r-aws_sns.tf#268) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.bootstrap_events]
- .aws_sns_topic.ca_cert_gen |(r-aws_sns.tf#163) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.ca_cert_gen]
- .aws_sns_topic.ca_commands |(r-aws_sns.tf#219) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.ca_commands]
- .aws_sns_topic.ca_events |(r-aws_sns.tf#100) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.ca_events]
- .aws_sns_topic.campaign_commands |(r-aws_sns.tf#30) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.campaign_commands]
- .aws_sns_topic.campaign_events |(r-aws_sns.tf#44) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.campaign_events]
- .aws_sns_topic.ci_commands |(r-aws_sns.tf#198) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.ci_commands]
- .aws_sns_topic.ci_events |(r-aws_sns.tf#205) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.ci_events]
- .aws_sns_topic.command_events |(r-aws_sns.tf#177) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.command_events]
- .aws_sns_topic.crypto_service_events |(r-aws_sns.tf#233) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.crypto_service_events]
- .aws_sns_topic.cryptographic_commands |(r-aws_sns.tf#142) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.cryptographic_commands]
- .aws_sns_topic.cryptographic_events |(r-aws_sns.tf#149) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.cryptographic_events]
- .aws_sns_topic.device_commands |(r-aws_sns.tf#107) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.device_commands]
- .aws_sns_topic.device_events |(r-aws_sns.tf#114) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.device_events]
- .aws_sns_topic.device_info |(r-aws_sns.tf#254) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.device_info]
- .aws_sns_topic.device_notifications |(r-aws_sns.tf#121) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.device_notifications]
- .aws_sns_topic.gp_ci_events |(r-aws_sns.tf#212) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.gp_ci_events]
- .aws_sns_topic.gp_commands |(r-aws_sns.tf#247) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.gp_commands]
- .aws_sns_topic.gp_cryptographic_events |(r-aws_sns.tf#226) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.gp_cryptographic_events]
- .aws_sns_topic.kcss_commands |(r-aws_sns.tf#240) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.kcss_commands]
- .aws_sns_topic.key_service_commands |(r-aws_sns.tf#16) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.key_service_commands]
- .aws_sns_topic.keys_commands |(r-aws_sns.tf#156) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.keys_commands]
- .aws_sns_topic.keys_events |(r-aws_sns.tf#23) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.keys_events]
- .aws_sns_topic.onboarding_events |(r-aws_sns.tf#51) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.onboarding_events]
- .aws_sns_topic.proxy_applet_commands |(r-aws_sns.tf#191) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.proxy_applet_commands]
- .aws_sns_topic.proxy_applet_device_commands |(r-aws_sns.tf#72) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.proxy_applet_device_commands]
- .aws_sns_topic.scheduled_events |(r-aws_sns.tf#2) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.scheduled_events]
- .aws_sns_topic.script_commands |(r-aws_sns.tf#79) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.script_commands]
- .aws_sns_topic.script_events |(r-aws_sns.tf#93) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.script_events]
- .aws_sns_topic.secure_messaging_events |(r-aws_sns.tf#261) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.secure_messaging_events]
- .aws_sns_topic.statistics_events |(r-aws_sns.tf#9) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.statistics_events]
- .aws_sns_topic.supported_commands |(r-aws_sns.tf#128) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.supported_commands]
- .aws_sns_topic.uicc |(r-aws_sns.tf#58) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.uicc]
- .aws_sns_topic.user_commands |(r-aws_sns.tf#170) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.user_commands]
- .aws_sns_topic.user_events |(r-aws_sns.tf#135) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.user_events]
- .aws_sns_topic.vendor_events |(r-aws_sns.tf#65) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic[aws_sns_topic.vendor_events]
- .aws_sns_topic_subscription.applet_events |(r-aws_sns.tf#395) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.applet_events]
- .aws_sns_topic_subscription.bootstrap_events |(r-aws_sns.tf#290) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.bootstrap_events]
- .aws_sns_topic_subscription.ca_cert_gen_events |(r-aws_sns.tf#283) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.ca_cert_gen_events]
- .aws_sns_topic_subscription.ca_commands |(r-aws_sns.tf#626) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.ca_commands]
- .aws_sns_topic_subscription.ca_events |(r-aws_sns.tf#367) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.ca_events]
- .aws_sns_topic_subscription.campaign_commands |(r-aws_sns.tf#297) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.campaign_commands]
- .aws_sns_topic_subscription.campaign_events |(r-aws_sns.tf#304) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.campaign_events]
- .aws_sns_topic_subscription.ci_commands |(r-aws_sns.tf#437) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.ci_commands]
- .aws_sns_topic_subscription.ci_events |(r-aws_sns.tf#444) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.ci_events]
- .aws_sns_topic_subscription.command_events |(r-aws_sns.tf#416) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.command_events]
- .aws_sns_topic_subscription.crypto_service_events |(r-aws_sns.tf#500) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.crypto_service_events]
- .aws_sns_topic_subscription.cryptographic_commands |(r-aws_sns.tf#388) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.cryptographic_commands]
- .aws_sns_topic_subscription.cryptographic_events |(r-aws_sns.tf#402) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.cryptographic_events]
- .aws_sns_topic_subscription.device_commands |(r-aws_sns.tf#332) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.device_commands]
- .aws_sns_topic_subscription.device_events |(r-aws_sns.tf#339) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.device_events]
- .aws_sns_topic_subscription.device_info |(r-aws_sns.tf#542) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.device_info]
- .aws_sns_topic_subscription.device_notifications |(r-aws_sns.tf#346) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.device_notifications]
- .aws_sns_topic_subscription.dg_user_commands |(r-aws_sns.tf#184) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.dg_user_commands]
- .aws_sns_topic_subscription.dg_vendor_events |(r-aws_sns.tf#458) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.dg_vendor_events]
- .aws_sns_topic_subscription.dim_command_events |(r-aws_sns.tf#423) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.dim_command_events]
- .aws_sns_topic_subscription.dim_device_events |(r-aws_sns.tf#430) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.dim_device_events]
- .aws_sns_topic_subscription.gp_ci_events |(r-aws_sns.tf#472) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.gp_ci_events]
- .aws_sns_topic_subscription.gp_commands |(r-aws_sns.tf#556) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.gp_commands]
- .aws_sns_topic_subscription.gp_cryptographic_events |(r-aws_sns.tf#479) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.gp_cryptographic_events]
- .aws_sns_topic_subscription.iccid_events |(r-aws_sns.tf#381) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.iccid_events]
- .aws_sns_topic_subscription.kcss_commands |(r-aws_sns.tf#514) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.kcss_commands]
- .aws_sns_topic_subscription.key_service_commands |(r-aws_sns.tf#507) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.key_service_commands]
- .aws_sns_topic_subscription.keys_commands |(r-aws_sns.tf#528) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.keys_commands]
- .aws_sns_topic_subscription.keys_commands_events |(r-aws_sns.tf#535) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.keys_commands_events]
- .aws_sns_topic_subscription.keys_events |(r-aws_sns.tf#521) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.keys_events]
- .aws_sns_topic_subscription.ks_uicc |(r-aws_sns.tf#570) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.ks_uicc]
- .aws_sns_topic_subscription.ks_uicc_user_events |(r-aws_sns.tf#563) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.ks_uicc_user_events]
- .aws_sns_topic_subscription.onboarding_events |(r-aws_sns.tf#577) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.onboarding_events]
- .aws_sns_topic_subscription.proxy_applet_commands |(r-aws_sns.tf#493) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.proxy_applet_commands]
- .aws_sns_topic_subscription.proxy_applet_device_commands |(r-aws_sns.tf#486) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.proxy_applet_device_commands]
- .aws_sns_topic_subscription.scheduled_events |(r-aws_sns.tf#276) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.scheduled_events]
- .aws_sns_topic_subscription.script_commands |(r-aws_sns.tf#311) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.script_commands]
- .aws_sns_topic_subscription.script_events |(r-aws_sns.tf#325) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.script_events]
- .aws_sns_topic_subscription.script_events_to_sqs_statistic_service |(r-aws_sns.tf#318) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.script_events_to_sqs_statistic_service]
- .aws_sns_topic_subscription.secure_messaging_events |(r-aws_sns.tf#549) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.secure_messaging_events]
- .aws_sns_topic_subscription.statistic_campaign_commands |(r-aws_sns.tf#612) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.statistic_campaign_commands]
- .aws_sns_topic_subscription.statistic_campaign_events |(r-aws_sns.tf#605) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.statistic_campaign_events]
- .aws_sns_topic_subscription.statistic_uicc |(r-aws_sns.tf#598) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.statistic_uicc]
- .aws_sns_topic_subscription.statistic_user_commands |(r-aws_sns.tf#591) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.statistic_user_commands]
- .aws_sns_topic_subscription.statistic_user_events |(r-aws_sns.tf#619) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.statistic_user_events]
- .aws_sns_topic_subscription.statistic_vendor_events |(r-aws_sns.tf#584) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.statistic_vendor_events]
- .aws_sns_topic_subscription.statistics_events |(r-aws_sns.tf#633) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.statistics_events]
- .aws_sns_topic_subscription.supported_commands |(r-aws_sns.tf#353) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.supported_commands]
- .aws_sns_topic_subscription.uicc |(r-aws_sns.tf#360) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.uicc]
- .aws_sns_topic_subscription.uicc_se_device_info |(r-aws_sns.tf#86) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.uicc_se_device_info]
- .aws_sns_topic_subscription.user_commands |(r-aws_sns.tf#409) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.user_commands]
- .aws_sns_topic_subscription.user_events |(r-aws_sns.tf#374) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.user_events]
- .aws_sns_topic_subscription.vendor_co_events |(r-aws_sns.tf#451) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.vendor_co_events]
- .aws_sns_topic_subscription.vendor_events |(r-aws_sns.tf#465) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription[aws_sns_topic_subscription.vendor_events]
## Resources-r-aws_sqs.tf
- .aws_sqs_queue.applet_events |(r-aws_sqs.tf#268) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.applet_events]
- .aws_sqs_queue.bootstrap_events |(r-aws_sqs.tf#182) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.bootstrap_events]
- .aws_sqs_queue.ca_cert_gen |(r-aws_sqs.tf#463) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.ca_cert_gen]
- .aws_sqs_queue.ca_commands |(r-aws_sqs.tf#718) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.ca_commands]
- .aws_sqs_queue.ca_events |(r-aws_sqs.tf#343) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.ca_events]
- .aws_sqs_queue.campaign_commands |(r-aws_sqs.tf#152) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.campaign_commands]
- .aws_sqs_queue.campaign_events |(r-aws_sqs.tf#197) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.campaign_events]
- .aws_sqs_queue.ci_commands |(r-aws_sqs.tf#553) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.ci_commands]
- .aws_sqs_queue.ci_events |(r-aws_sqs.tf#538) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.ci_events]
- .aws_sqs_queue.command_events |(r-aws_sqs.tf#628) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.command_events]
- .aws_sqs_queue.crypto_service_events |(r-aws_sqs.tf#508) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.crypto_service_events]
- .aws_sqs_queue.cryptographic_commands |(r-aws_sqs.tf#433) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.cryptographic_commands]
- .aws_sqs_queue.cryptographic_events |(r-aws_sqs.tf#448) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.cryptographic_events]
- .aws_sqs_queue.dead_letter |(r-aws_sqs.tf#212) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.dead_letter]
- .aws_sqs_queue.device_commands |(r-aws_sqs.tf#253) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.device_commands]
- .aws_sqs_queue.device_events |(r-aws_sqs.tf#298) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.device_events]
- .aws_sqs_queue.device_info_events |(r-aws_sqs.tf#673) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.device_info_events]
- .aws_sqs_queue.device_notifications |(r-aws_sqs.tf#313) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.device_notifications]
- .aws_sqs_queue.device_onboard |(r-aws_sqs.tf#328) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.device_onboard]
- .aws_sqs_queue.dg_user_commands |(r-aws_sqs.tf#77) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.dg_user_commands]
- .aws_sqs_queue.dg_vendor_events |(r-aws_sqs.tf#92) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.dg_vendor_events]
- .aws_sqs_queue.dim_command_events |(r-aws_sqs.tf#643) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.dim_command_events]
- .aws_sqs_queue.dim_device_events |(r-aws_sqs.tf#658) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.dim_device_events]
- .aws_sqs_queue.gp_ci_events |(r-aws_sqs.tf#568) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.gp_ci_events]
- .aws_sqs_queue.gp_commands |(r-aws_sqs.tf#703) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.gp_commands]
- .aws_sqs_queue.gp_cryptographic_events |(r-aws_sqs.tf#598) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.gp_cryptographic_events]
- .aws_sqs_queue.iccid_events |(r-aws_sqs.tf#283) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.iccid_events]
- .aws_sqs_queue.kcss_commands |(r-aws_sqs.tf#523) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.kcss_commands]
- .aws_sqs_queue.key_service_events |(r-aws_sqs.tf#2) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.key_service_events]
- .aws_sqs_queue.keys_commands |(r-aws_sqs.tf#62) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.keys_commands]
- .aws_sqs_queue.keys_events |(r-aws_sqs.tf#32) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.keys_events]
- .aws_sqs_queue.ks_uicc |(r-aws_sqs.tf#107) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.ks_uicc]
- .aws_sqs_queue.proxy_applet_device_command_events |(r-aws_sqs.tf#373) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.proxy_applet_device_command_events]
- .aws_sqs_queue.scheduled_events |(r-aws_sqs.tf#17) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.scheduled_events]
- .aws_sqs_queue.scheduled_events_commands |(r-aws_sqs.tf#613) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.scheduled_events_commands]
- .aws_sqs_queue.script_commands |(r-aws_sqs.tf#223) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.script_commands]
- .aws_sqs_queue.script_events |(r-aws_sqs.tf#238) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.script_events]
- .aws_sqs_queue.se_device_info |(r-aws_sqs.tf#583) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.se_device_info]
- .aws_sqs_queue.se_events |(r-aws_sqs.tf#388) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.se_events]
- .aws_sqs_queue.se_status |(r-aws_sqs.tf#358) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.se_status]
- .aws_sqs_queue.secure_messaging_events |(r-aws_sqs.tf#688) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.secure_messaging_events]
- .aws_sqs_queue.sms_events |(r-aws_sqs.tf#47) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.sms_events]
- .aws_sqs_queue.statistics_events |(r-aws_sqs.tf#493) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.statistics_events]
- .aws_sqs_queue.supported_commands |(r-aws_sqs.tf#403) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.supported_commands]
- .aws_sqs_queue.uicc |(r-aws_sqs.tf#167) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.uicc]
- .aws_sqs_queue.user_commands |(r-aws_sqs.tf#478) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.user_commands]
- .aws_sqs_queue.user_events |(r-aws_sqs.tf#418) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.user_events]
- .aws_sqs_queue.vendor_co_events |(r-aws_sqs.tf#122) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.vendor_co_events]
- .aws_sqs_queue.vendor_events |(r-aws_sqs.tf#137) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue[aws_sqs_queue.vendor_events]
- .aws_sqs_queue_policy.proxy_applet_device_command_events |(r-aws_sqs.tf#998) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.proxy_applet_device_command_events]
- .aws_sqs_queue_policy.sqs_policy_for_device_info_events |(r-aws_sqs.tf#1070) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_device_info_events]
- .aws_sqs_queue_policy.sqs_policy_for_iccid_events |(r-aws_sqs.tf#979) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_iccid_events]
- .aws_sqs_queue_policy.sqs_policy_for_secure_messaging_events |(r-aws_sqs.tf#1079) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_secure_messaging_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_applet_events |(r-aws_sqs.tf#762) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_applet_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_bootstrap_events |(r-aws_sqs.tf#798) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_bootstrap_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_ca_cert_gen |(r-aws_sqs.tf#1025) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_ca_cert_gen]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_ca_commands |(r-aws_sqs.tf#1152) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_ca_commands]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_ca_events |(r-aws_sqs.tf#844) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_ca_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_campaign_commands |(r-aws_sqs.tf#753) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_campaign_commands]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_campaign_events |(r-aws_sqs.tf#825) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_campaign_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_ci_commands |(r-aws_sqs.tf#816) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_ci_commands]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_ci_events |(r-aws_sqs.tf#1106) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_ci_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_command_events |(r-aws_sqs.tf#906) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_command_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_crypto_service_events |(r-aws_sqs.tf#862) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_crypto_service_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_cryptographic_commands |(r-aws_sqs.tf#1016) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_cryptographic_commands]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_cryptographic_events |(r-aws_sqs.tf#1034) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_cryptographic_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_device_commands |(r-aws_sqs.tf#871) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_device_commands]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_device_events |(r-aws_sqs.tf#933) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_device_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_device_notifications |(r-aws_sqs.tf#1124) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_device_notifications]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_device_onboard |(r-aws_sqs.tf#942) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_device_onboard]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_dg_user_commands |(r-aws_sqs.tf#897) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_dg_user_commands]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_dg_vendor_events |(r-aws_sqs.tf#1061) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_dg_vendor_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_dim_command_events |(r-aws_sqs.tf#915) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_dim_command_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_dim_device_events |(r-aws_sqs.tf#924) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_dim_device_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_gp_ci_events |(r-aws_sqs.tf#1097) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_gp_ci_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_gp_commands |(r-aws_sqs.tf#1088) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_gp_commands]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_gp_cryptographic_events |(r-aws_sqs.tf#1115) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_gp_cryptographic_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_kcss_commands |(r-aws_sqs.tf#807) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_kcss_commands]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_key_service_events |(r-aws_sqs.tf#780) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_key_service_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_keys_commands |(r-aws_sqs.tf#1143) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_keys_commands]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_keys_events |(r-aws_sqs.tf#1133) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_keys_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_ks_uicc |(r-aws_sqs.tf#743) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_ks_uicc]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_scheduled_events |(r-aws_sqs.tf#734) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_scheduled_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_scheduled_events_commands |(r-aws_sqs.tf#889) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_scheduled_events_commands]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_script_commands |(r-aws_sqs.tf#835) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_script_commands]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_script_events |(r-aws_sqs.tf#853) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_script_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_se_device_info |(r-aws_sqs.tf#960) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_se_device_info]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_se_events |(r-aws_sqs.tf#969) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_se_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_se_status |(r-aws_sqs.tf#951) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_se_status]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_sms_events |(r-aws_sqs.tf#789) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_sms_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_statistics_events |(r-aws_sqs.tf#1161) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_statistics_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_supported_commands |(r-aws_sqs.tf#989) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_supported_commands]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_uicc |(r-aws_sqs.tf#771) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_uicc]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_user_commands |(r-aws_sqs.tf#880) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_user_commands]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_user_events |(r-aws_sqs.tf#1007) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_user_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_vendor_co_events |(r-aws_sqs.tf#1043) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_vendor_co_events]
- .aws_sqs_queue_policy.sqs_policy_for_sqs_vendor_events |(r-aws_sqs.tf#1052) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy[aws_sqs_queue_policy.sqs_policy_for_sqs_vendor_events]
## Resources-r-aws_network.tf
- .aws_subnet.private_1 |(r-aws_network.tf#118) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet[aws_subnet.private_1]
- .aws_subnet.private_2 |(r-aws_network.tf#132) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet[aws_subnet.private_2]
- .aws_subnet.private_3 |(r-aws_network.tf#146) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet[aws_subnet.private_3]
- .aws_subnet.public_1 |(r-aws_network.tf#76) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet[aws_subnet.public_1]
- .aws_subnet.public_2 |(r-aws_network.tf#90) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet[aws_subnet.public_2]
- .aws_subnet.public_3 |(r-aws_network.tf#104) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet[aws_subnet.public_3]
- .aws_vpc.this |(r-aws_network.tf#2) |resource |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/vpc[aws_vpc.this]
## Resources-r-aws_kubernetes.tf
- .local_file.config |(r-aws_kubernetes.tf#175) |resource |https://registry.terraform.io/providers/hashicorp/local/latest/docs/resources/file[local_file.config]
- .local_file.configmap |(r-aws_kubernetes.tf#170) |resource |https://registry.terraform.io/providers/hashicorp/local/latest/docs/resources/file[local_file.configmap]
- .null_resource.apply_config_map_aws_auth_yaml |(r-aws_kubernetes.tf#185) |resource |https://registry.terraform.io/providers/hashicorp/null/latest/docs/resources/resource[null_resource.apply_config_map_aws_auth_yaml]
- .null_resource.pre_setup |(r-aws_kubernetes.tf#1) |resource |https://registry.terraform.io/providers/hashicorp/null/latest/docs/resources/resource[null_resource.pre_setup]
## Resources-r-aws_openldap.tf
- .random_string.openldap_admin_passwd |(r-aws_openldap.tf#2) |resource |https://registry.terraform.io/providers/hashicorp/random/latest/docs/resources/string[random_string.openldap_admin_passwd]
## Resources-r-aws_lambda_dynamodb_backup.tf
- .archive_file.dynamo_db_backup_zip |(r-aws_lambda_dynamodb_backup.tf#42) |data source |https://registry.terraform.io/providers/hashicorp/archive/latest/docs/data-sources/file[archive_file.dynamo_db_backup_zip]
## Resources-data.tf
- .aws_ami.amazon-linux-2 |(data.tf#31) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/ami[aws_ami.amazon-linux-2]
- .aws_ami.centos7 |(data.tf#14) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/ami[aws_ami.centos7]
- .aws_ami.centos7-ldap |(data.tf#53) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/ami[aws_ami.centos7-ldap]
- .aws_ami.eks-node |(data.tf#44) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/ami[aws_ami.eks-node]
- .aws_ami.ubuntu |(data.tf#1) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/ami[aws_ami.ubuntu]
- .aws_caller_identity.current |(data.tf#72) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/caller_identity[aws_caller_identity.current]
- .aws_iam_policy_document.eks-cluster-autoscaler |(data.tf#388) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document[aws_iam_policy_document.eks-cluster-autoscaler]
- .aws_iam_policy_document.prometheus |(data.tf#406) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document[aws_iam_policy_document.prometheus]
- .aws_iam_policy_document.vsts-bootstrap-service |(data.tf#298) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document[aws_iam_policy_document.vsts-bootstrap-service]
- .aws_iam_policy_document.vsts-campaign-orchestrator |(data.tf#81) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document[aws_iam_policy_document.vsts-campaign-orchestrator]
- .aws_iam_policy_document.vsts-ci-service |(data.tf#99) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document[aws_iam_policy_document.vsts-ci-service]
- .aws_iam_policy_document.vsts-content-service |(data.tf#117) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document[aws_iam_policy_document.vsts-content-service]
- .aws_iam_policy_document.vsts-crypto-service |(data.tf#135) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document[aws_iam_policy_document.vsts-crypto-service]
- .aws_iam_policy_document.vsts-device-gateway |(data.tf#262) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document[aws_iam_policy_document.vsts-device-gateway]
- .aws_iam_policy_document.vsts-dim-service |(data.tf#225) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document[aws_iam_policy_document.vsts-dim-service]
- .aws_iam_policy_document.vsts-event-scheduler |(data.tf#153) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document[aws_iam_policy_document.vsts-event-scheduler]
- .aws_iam_policy_document.vsts-gp-service |(data.tf#280) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document[aws_iam_policy_document.vsts-gp-service]
- .aws_iam_policy_document.vsts-kcss-service |(data.tf#171) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document[aws_iam_policy_document.vsts-kcss-service]
- .aws_iam_policy_document.vsts-key-service |(data.tf#244) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document[aws_iam_policy_document.vsts-key-service]
- .aws_iam_policy_document.vsts-notification-service |(data.tf#316) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document[aws_iam_policy_document.vsts-notification-service]
- .aws_iam_policy_document.vsts-proxy-applet-service |(data.tf#352) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document[aws_iam_policy_document.vsts-proxy-applet-service]
- .aws_iam_policy_document.vsts-script-executor |(data.tf#189) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document[aws_iam_policy_document.vsts-script-executor]
- .aws_iam_policy_document.vsts-sms-service |(data.tf#370) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document[aws_iam_policy_document.vsts-sms-service]
- .aws_iam_policy_document.vsts-statistic-service |(data.tf#334) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document[aws_iam_policy_document.vsts-statistic-service]
- .aws_iam_policy_document.vsts-user-service |(data.tf#207) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document[aws_iam_policy_document.vsts-user-service]
- .aws_iot_endpoint.current |(data.tf#74) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iot_endpoint[aws_iot_endpoint.current]
- .aws_region.current |(data.tf#70) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/region[aws_region.current]
- .aws_route53_zone.default |(data.tf#76) |data source |https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/route53_zone[aws_route53_zone.default]
- .external_external.oidc-thumbprint |(data.tf#424) |data source |https://registry.terraform.io/providers/hashicorp/external/latest/docs/data-sources/external[external_external.oidc-thumbprint]
<!-- END_TF_DOCS -->