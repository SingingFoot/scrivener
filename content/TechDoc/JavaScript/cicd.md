+++
title = "CICD"
description = "This is an area for technical documentation"
weight = 3
+++


## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 0.13.0, <= 0.13.3 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | ~> 2.7 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_archive"></a> [archive](#provider\_archive) | n/a |
| <a name="provider_aws"></a> [aws](#provider\_aws) | ~> 2.7 |
| <a name="provider_external"></a> [external](#provider\_external) | n/a |
| <a name="provider_local"></a> [local](#provider\_local) | n/a |
| <a name="provider_null"></a> [null](#provider\_null) | n/a |
| <a name="provider_random"></a> [random](#provider\_random) | n/a |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_acm_certificate.api-gateway-cert](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/acm_certificate) | resource |
| [aws_acm_certificate.openldap](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/acm_certificate) | resource |
| [aws_acm_certificate.wildcard](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/acm_certificate) | resource |
| [aws_acm_certificate_validation.api-gateway-valid](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/acm_certificate_validation) | resource |
| [aws_acm_certificate_validation.openldap](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/acm_certificate_validation) | resource |
| [aws_acm_certificate_validation.wildcard](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/acm_certificate_validation) | resource |
| [aws_api_gateway_authorizer.lambda-authorizer](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_authorizer) | resource |
| [aws_api_gateway_base_path_mapping.dev](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_base_path_mapping) | resource |
| [aws_api_gateway_deployment.deployment](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_deployment) | resource |
| [aws_api_gateway_domain_name.api-gateway-domain](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_domain_name) | resource |
| [aws_api_gateway_gateway_response.access_denied](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_gateway_response) | resource |
| [aws_api_gateway_gateway_response.missing_authentication_token](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_gateway_response) | resource |
| [aws_api_gateway_gateway_response.resource_not_found](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_gateway_response) | resource |
| [aws_api_gateway_gateway_response.unauthorized](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_gateway_response) | resource |
| [aws_api_gateway_integration.api-method-integration-content-proxy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration) | resource |
| [aws_api_gateway_integration.api-method-integration-oauth-proxy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration) | resource |
| [aws_api_gateway_integration.api-method-integration-users-proxy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration) | resource |
| [aws_api_gateway_integration.cors_content_integration](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration) | resource |
| [aws_api_gateway_integration.cors_oauth_integration](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration) | resource |
| [aws_api_gateway_integration.cors_oauth_validate](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration) | resource |
| [aws_api_gateway_integration.cors_oauth_validate_auth](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration) | resource |
| [aws_api_gateway_integration.cors_oauth_validate_auth_integration](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration) | resource |
| [aws_api_gateway_integration.cors_oauth_validate_integration](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration) | resource |
| [aws_api_gateway_integration.cors_users_integration](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration) | resource |
| [aws_api_gateway_integration_response.cors_integration_content_response](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration_response) | resource |
| [aws_api_gateway_integration_response.cors_integration_oauth_options_response](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration_response) | resource |
| [aws_api_gateway_integration_response.cors_integration_oauth_options_response_auth](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration_response) | resource |
| [aws_api_gateway_integration_response.cors_integration_oauth_response](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration_response) | resource |
| [aws_api_gateway_integration_response.cors_integration_oauth_validate_auth_response](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration_response) | resource |
| [aws_api_gateway_integration_response.cors_integration_oauth_validate_response](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration_response) | resource |
| [aws_api_gateway_integration_response.cors_integration_users_response](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_integration_response) | resource |
| [aws_api_gateway_method.api-method-content-proxy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method) | resource |
| [aws_api_gateway_method.api-method-oauth-proxy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method) | resource |
| [aws_api_gateway_method.api-method-oauth-validate](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method) | resource |
| [aws_api_gateway_method.api-method-oauth-validate-auth](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method) | resource |
| [aws_api_gateway_method.api-method-user-proxy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method) | resource |
| [aws_api_gateway_method.cors_method_content](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method) | resource |
| [aws_api_gateway_method.cors_method_oauth](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method) | resource |
| [aws_api_gateway_method.cors_method_oauth_validate](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method) | resource |
| [aws_api_gateway_method.cors_method_oauth_validate_auth](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method) | resource |
| [aws_api_gateway_method.cors_method_users](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method) | resource |
| [aws_api_gateway_method_response.content-service-response-401](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response) | resource |
| [aws_api_gateway_method_response.content-service-response-403](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response) | resource |
| [aws_api_gateway_method_response.cors_method_content_response](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response) | resource |
| [aws_api_gateway_method_response.cors_method_oauth_options_validate](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response) | resource |
| [aws_api_gateway_method_response.cors_method_oauth_options_validate_auth](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response) | resource |
| [aws_api_gateway_method_response.cors_method_oauth_response](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response) | resource |
| [aws_api_gateway_method_response.cors_method_oauth_validate](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response) | resource |
| [aws_api_gateway_method_response.cors_method_oauth_validate_auth](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response) | resource |
| [aws_api_gateway_method_response.cors_method_users_response](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response) | resource |
| [aws_api_gateway_method_response.user-service-response-401](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response) | resource |
| [aws_api_gateway_method_response.user-service-response-403](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_method_response) | resource |
| [aws_api_gateway_resource.content-proxy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_resource) | resource |
| [aws_api_gateway_resource.content-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_resource) | resource |
| [aws_api_gateway_resource.oauth-keycloak](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_resource) | resource |
| [aws_api_gateway_resource.oauth-proxy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_resource) | resource |
| [aws_api_gateway_resource.oauth-validate](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_resource) | resource |
| [aws_api_gateway_resource.oauth-validate-auth](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_resource) | resource |
| [aws_api_gateway_resource.user-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_resource) | resource |
| [aws_api_gateway_resource.users-proxy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_resource) | resource |
| [aws_api_gateway_rest_api.api](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_rest_api) | resource |
| [aws_api_gateway_vpc_link.api-gateway](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/api_gateway_vpc_link) | resource |
| [aws_autoscaling_group.eks_node](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/autoscaling_group) | resource |
| [aws_autoscaling_policy.eks_node_policy_down](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/autoscaling_policy) | resource |
| [aws_autoscaling_policy.eks_node_policy_up](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/autoscaling_policy) | resource |
| [aws_cloudwatch_event_rule.function_check](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_event_rule) | resource |
| [aws_cloudwatch_event_rule.schedule-dynamodb-backup](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_event_rule) | resource |
| [aws_cloudwatch_event_rule.schedule-es-cleanup-lambda](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_event_rule) | resource |
| [aws_cloudwatch_event_target.check_lambda_function](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_event_target) | resource |
| [aws_cloudwatch_event_target.dynamodb_backup](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_event_target) | resource |
| [aws_cloudwatch_event_target.es_cleanup](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_event_target) | resource |
| [aws_cloudwatch_log_group.cwlog](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_log_group) | resource |
| [aws_cloudwatch_metric_alarm.eks_node_cpu_alarm_down](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_metric_alarm) | resource |
| [aws_cloudwatch_metric_alarm.eks_node_cpu_alarm_up](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_metric_alarm) | resource |
| [aws_cloudwatch_metric_alarm.es-disk](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_metric_alarm) | resource |
| [aws_cloudwatch_metric_alarm.es-disk-statistic](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_metric_alarm) | resource |
| [aws_default_route_table.default](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/default_route_table) | resource |
| [aws_default_security_group.default](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/default_security_group) | resource |
| [aws_dynamodb_table.applet](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.bs_iccid_info](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.campaign](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.campaign_execution](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.co_campaign_execution](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.co_script_execution](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.co_vendor](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.cs_api_key](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.cs_campaign_execution](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.cs_ce_command_execution](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.cs_grouped_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.cs_script_execution](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.cs_vendor_permissions](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.custom_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.device_command](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.device_config_links](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.device_info](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.device_notifications](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.dg_api_key](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.dg_vendor](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.es_user_info](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.es_vendor_info](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.gp_applet](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.gp_command_preparation](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.group](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.iccid](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.identities](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.kcss_command_preparation](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.ks_iccid_info](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.pa_applet_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.proxy_applet_session_info](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.relation_profile](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.role](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.scheduled_event](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.script](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.script_execution](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.script_template](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.se_device_info](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.supported_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.uicc](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.uicc_group](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.us_api_key](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.us_supported_ca](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.user](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_dynamodb_table.vendor](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_efs_file_system.efs_key_service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/efs_file_system) | resource |
| [aws_efs_file_system_policy.policy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/efs_file_system_policy) | resource |
| [aws_efs_mount_target.efs_key_service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/efs_mount_target) | resource |
| [aws_eip.eip_1](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip) | resource |
| [aws_eip.eip_2](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip) | resource |
| [aws_eip.eip_3_proxy_applet](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip) | resource |
| [aws_eip_association.infrastructure_bastion_eip_association](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip_association) | resource |
| [aws_eks_cluster.cluster](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eks_cluster) | resource |
| [aws_elasticsearch_domain.es_apps_logs_storage](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/elasticsearch_domain) | resource |
| [aws_elasticsearch_domain.es_apps_logs_storage_statistic](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/elasticsearch_domain) | resource |
| [aws_iam_access_key.backup_user](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_access_key) | resource |
| [aws_iam_access_key.mail_sender_user](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_access_key) | resource |
| [aws_iam_instance_profile.eks-instance](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_instance_profile) | resource |
| [aws_iam_openid_connect_provider.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_openid_connect_provider) | resource |
| [aws_iam_policy.backup_user](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.eks-albingress](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.eks-albingress-dns](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.eks-cluster-autoscaler](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.grafana-datasource-cloudwatch](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.kms_full_access](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.lambda_es_access](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.prometheus](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.ses](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.vsts-bootstrap-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.vsts-campaign-orchestrator](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.vsts-ci-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.vsts-content-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.vsts-crypto-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.vsts-device-gateway](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.vsts-dim-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.vsts-event-scheduler](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.vsts-gp-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.vsts-kcss-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.vsts-key-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.vsts-notification-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.vsts-proxy-applet-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.vsts-script-executor](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.vsts-sms-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.vsts-statistic-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy.vsts-user-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_policy_attachment.attach_eks-albingress](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy_attachment) | resource |
| [aws_iam_policy_attachment.attach_eks-albingress-dns](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy_attachment) | resource |
| [aws_iam_role.device_onboard](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.dynamo_db_backup](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.eks](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.eks-cluster-autoscaler](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.eks-instance](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.invocation_role](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.lambda-api-gateway](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.openldap_dlm_lifecycle_role](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.prometheus](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.se_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.se_status](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.vsts-bootstrap-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.vsts-campaign-orchestrator](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.vsts-ci-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.vsts-content-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.vsts-crypto-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.vsts-device-gateway](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.vsts-dim-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.vsts-event-scheduler](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.vsts-gp-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.vsts-kcss-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.vsts-key-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.vsts-notification-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.vsts-proxy-applet-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.vsts-script-executor](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.vsts-sms-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.vsts-statistic-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.vsts-user-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.vsts_lambda_db_campaign_execution](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.vsts_lambda_es_cleanup](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role_policy.device_onboard](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy) | resource |
| [aws_iam_role_policy.invocation_policy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy) | resource |
| [aws_iam_role_policy.openldap_dlm_lifecycle_role_policy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy) | resource |
| [aws_iam_role_policy.se_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy) | resource |
| [aws_iam_role_policy.se_status](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy) | resource |
| [aws_iam_role_policy_attachment.AmazonDynamoDBFullAccess](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.AmazonDynamoDBFullAccess_dynamod_backup](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.AmazonSNSFullAccess](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.CloudWatchFullAccess](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.CloudWatchFullAccess-lambda-api-gateway](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.CloudWatchFullAccess_dynamod_backup](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.KMSFullAccess](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.KMSFullAccess_dynamod_backup](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.eks-AmazonEKSClusterPolicy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.eks-AmazonEKSServicePolicy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.eks-cluster-autoscaler](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.eks-instance-AmazonCloudwatchGrafana](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.eks-instance-AmazonEC2ContainerRegistryReadOnly](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.eks-instance-AmazonEKSWorkerNodePolicy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.eks-instance-AmazonEKS_CNI_Policy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.lambda-es-permission](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.prometheus](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.vsts-bootstrap-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.vsts-campaign-orchestrator](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.vsts-ci-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.vsts-content-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.vsts-crypto-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.vsts-device-gateway](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.vsts-dim-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.vsts-event-scheduler](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.vsts-gp-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.vsts-kcss-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.vsts-key-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.vsts-notification-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.vsts-proxy-applet-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.vsts-script-executor](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.vsts-sms-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.vsts-statistic-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.vsts-user-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_user.backup_user](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_user) | resource |
| [aws_iam_user.mail_sender_user](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_user) | resource |
| [aws_iam_user_policy_attachment.backup_user](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_user_policy_attachment) | resource |
| [aws_iam_user_policy_attachment.ses](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_user_policy_attachment) | resource |
| [aws_instance.bastion](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/instance) | resource |
| [aws_instance.openldap](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/instance) | resource |
| [aws_internet_gateway.igw_1](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/internet_gateway) | resource |
| [aws_iot_certificate.cert_thing_backend_client](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_certificate) | resource |
| [aws_iot_certificate.cert_thing_bootstrap](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_certificate) | resource |
| [aws_iot_policy.policy_thing](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_policy) | resource |
| [aws_iot_policy.policy_thing_backend_client](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_policy) | resource |
| [aws_iot_policy.policy_thing_bootstrap](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_policy) | resource |
| [aws_iot_policy_attachment.policy_thing_attachment](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_policy_attachment) | resource |
| [aws_iot_policy_attachment.policy_thing_backend_client_attachment](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_policy_attachment) | resource |
| [aws_iot_policy_attachment.policy_thing_bootstrap_attachment](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_policy_attachment) | resource |
| [aws_iot_thing.thing_backend_client](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_thing) | resource |
| [aws_iot_thing.thing_bootstrap](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_thing) | resource |
| [aws_iot_thing_principal_attachment.principal_thing_backend_client_attachment](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_thing_principal_attachment) | resource |
| [aws_iot_thing_principal_attachment.principal_thing_bootstrap_attachment](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_thing_principal_attachment) | resource |
| [aws_iot_thing_type.type1](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_thing_type) | resource |
| [aws_iot_topic_rule.device_onboard](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_topic_rule) | resource |
| [aws_iot_topic_rule.se_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_topic_rule) | resource |
| [aws_iot_topic_rule.se_status](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iot_topic_rule) | resource |
| [aws_key_pair.eks-node](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/key_pair) | resource |
| [aws_kms_alias.common_key](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/kms_alias) | resource |
| [aws_kms_key.common_key](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/kms_key) | resource |
| [aws_lambda_event_source_mapping.lambda-db-campaign-execution-trigger](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_event_source_mapping) | resource |
| [aws_lambda_function.authorizer](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_function) | resource |
| [aws_lambda_function.db-campaign-execution](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_function) | resource |
| [aws_lambda_function.dynamodb-backup](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_function) | resource |
| [aws_lambda_function.vsts_es_cleanup](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_function) | resource |
| [aws_lambda_permission.allow_cloudwatch](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_permission) | resource |
| [aws_lambda_permission.allow_cloudwatch_dynamod_backup](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_permission) | resource |
| [aws_lambda_permission.allow_cloudwatch_to_call_function](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_permission) | resource |
| [aws_launch_configuration.eks_node](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/launch_configuration) | resource |
| [aws_lb.load_balancer](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb) | resource |
| [aws_lb.load_balancer_proxy_applet](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb) | resource |
| [aws_lb.openldap](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb) | resource |
| [aws_lb.wireguard_lb](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb) | resource |
| [aws_lb_listener.listener](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_listener) | resource |
| [aws_lb_listener.listener-proxy-applet](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_listener) | resource |
| [aws_lb_listener.openldap_port443](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_listener) | resource |
| [aws_lb_listener.openldap_port80](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_listener) | resource |
| [aws_lb_listener.wireguard_listener](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_listener) | resource |
| [aws_lb_target_group.nlb-tg](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_target_group) | resource |
| [aws_lb_target_group.nlb-tg-proxy-applet](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_target_group) | resource |
| [aws_lb_target_group.openldap](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_target_group) | resource |
| [aws_lb_target_group.wireguard-tg](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_target_group) | resource |
| [aws_lb_target_group_attachment.openldap](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_target_group_attachment) | resource |
| [aws_nat_gateway.natgw_1](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/nat_gateway) | resource |
| [aws_route53_record.api-gateway](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route53_record) | resource |
| [aws_route53_record.api_gateway_cert_validation](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route53_record) | resource |
| [aws_route53_record.openldap](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route53_record) | resource |
| [aws_route53_record.openldap_cert_validation](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route53_record) | resource |
| [aws_route53_record.storage-documentation](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route53_record) | resource |
| [aws_route53_record.wildcard_cert_validation](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route53_record) | resource |
| [aws_route53_record.wireguard](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route53_record) | resource |
| [aws_route_table.private](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table) | resource |
| [aws_route_table.public](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table) | resource |
| [aws_route_table_association.private_1](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.private_2](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.private_3](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.public_1](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.public_2](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.public_3](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_s3_bucket.backup_bucket](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket) | resource |
| [aws_s3_bucket.ca-certificates](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket) | resource |
| [aws_s3_bucket.campaign-execution](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket) | resource |
| [aws_s3_bucket.device-configuration](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket) | resource |
| [aws_s3_bucket.dim-certificate](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket) | resource |
| [aws_s3_bucket.prometheus](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket) | resource |
| [aws_s3_bucket.static-site-documentation](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket) | resource |
| [aws_s3_bucket_object.openldap_backup_folder](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket_object) | resource |
| [aws_s3_bucket_policy.static-site-documentation_policy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket_policy) | resource |
| [aws_security_group.efs-sg](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group) | resource |
| [aws_security_group.eks](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group) | resource |
| [aws_security_group.eks-node](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group) | resource |
| [aws_security_group.eks-node-test](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group) | resource |
| [aws_security_group.es_cleanup](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group) | resource |
| [aws_security_group.openldap_alb](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group) | resource |
| [aws_security_group.openldap_ec2](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group) | resource |
| [aws_security_group.sg_bastion](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group) | resource |
| [aws_security_group.sg_common](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group) | resource |
| [aws_security_group.sg_es](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group) | resource |
| [aws_security_group_rule.http](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group_rule) | resource |
| [aws_security_group_rule.ingress-eks](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group_rule) | resource |
| [aws_security_group_rule.ingress-node-https](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group_rule) | resource |
| [aws_security_group_rule.ingress-self](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group_rule) | resource |
| [aws_security_group_rule.ingress-workstation-https](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group_rule) | resource |
| [aws_ses_email_identity.mail_sender_user](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ses_email_identity) | resource |
| [aws_sns_platform_application.fcm_application](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_platform_application) | resource |
| [aws_sns_topic.applet_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.bootstrap_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.ca_cert_gen](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.ca_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.ca_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.campaign_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.campaign_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.ci_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.ci_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.command_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.crypto_service_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.cryptographic_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.cryptographic_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.device_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.device_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.device_info](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.device_notifications](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.gp_ci_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.gp_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.gp_cryptographic_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.kcss_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.key_service_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.keys_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.keys_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.onboarding_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.proxy_applet_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.proxy_applet_device_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.scheduled_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.script_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.script_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.secure_messaging_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.statistics_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.supported_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.uicc](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.user_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.user_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic.vendor_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic) | resource |
| [aws_sns_topic_subscription.applet_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.bootstrap_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.ca_cert_gen_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.ca_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.ca_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.campaign_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.campaign_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.ci_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.ci_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.command_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.crypto_service_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.cryptographic_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.cryptographic_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.device_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.device_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.device_info](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.device_notifications](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.dg_user_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.dg_vendor_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.dim_command_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.dim_device_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.gp_ci_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.gp_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.gp_cryptographic_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.iccid_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.kcss_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.key_service_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.keys_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.keys_commands_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.keys_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.ks_uicc](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.ks_uicc_user_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.onboarding_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.proxy_applet_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.proxy_applet_device_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.scheduled_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.script_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.script_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.script_events_to_sqs_statistic_service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.secure_messaging_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.statistic_campaign_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.statistic_campaign_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.statistic_uicc](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.statistic_user_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.statistic_user_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.statistic_vendor_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.statistics_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.supported_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.uicc](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.uicc_se_device_info](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.user_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.user_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.vendor_co_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sns_topic_subscription.vendor_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sns_topic_subscription) | resource |
| [aws_sqs_queue.applet_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.bootstrap_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.ca_cert_gen](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.ca_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.ca_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.campaign_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.campaign_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.ci_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.ci_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.command_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.crypto_service_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.cryptographic_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.cryptographic_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.dead_letter](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.device_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.device_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.device_info_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.device_notifications](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.device_onboard](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.dg_user_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.dg_vendor_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.dim_command_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.dim_device_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.gp_ci_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.gp_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.gp_cryptographic_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.iccid_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.kcss_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.key_service_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.keys_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.keys_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.ks_uicc](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.proxy_applet_device_command_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.scheduled_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.scheduled_events_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.script_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.script_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.se_device_info](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.se_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.se_status](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.secure_messaging_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.sms_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.statistics_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.supported_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.uicc](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.user_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.user_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.vendor_co_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue.vendor_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue) | resource |
| [aws_sqs_queue_policy.proxy_applet_device_command_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_device_info_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_iccid_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_secure_messaging_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_applet_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_bootstrap_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_ca_cert_gen](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_ca_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_ca_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_campaign_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_campaign_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_ci_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_ci_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_command_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_crypto_service_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_cryptographic_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_cryptographic_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_device_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_device_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_device_notifications](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_device_onboard](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_dg_user_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_dg_vendor_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_dim_command_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_dim_device_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_gp_ci_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_gp_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_gp_cryptographic_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_kcss_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_key_service_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_keys_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_keys_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_ks_uicc](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_scheduled_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_scheduled_events_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_script_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_script_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_se_device_info](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_se_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_se_status](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_sms_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_statistics_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_supported_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_uicc](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_user_commands](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_user_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_vendor_co_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_sqs_queue_policy.sqs_policy_for_sqs_vendor_events](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sqs_queue_policy) | resource |
| [aws_subnet.private_1](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.private_2](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.private_3](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.public_1](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.public_2](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.public_3](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_vpc.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/vpc) | resource |
| [local_file.config](https://registry.terraform.io/providers/hashicorp/local/latest/docs/resources/file) | resource |
| [local_file.configmap](https://registry.terraform.io/providers/hashicorp/local/latest/docs/resources/file) | resource |
| [null_resource.apply_config_map_aws_auth_yaml](https://registry.terraform.io/providers/hashicorp/null/latest/docs/resources/resource) | resource |
| [null_resource.pre_setup](https://registry.terraform.io/providers/hashicorp/null/latest/docs/resources/resource) | resource |
| [random_string.openldap_admin_passwd](https://registry.terraform.io/providers/hashicorp/random/latest/docs/resources/string) | resource |
| [archive_file.dynamo_db_backup_zip](https://registry.terraform.io/providers/hashicorp/archive/latest/docs/data-sources/file) | data source |
| [aws_ami.amazon-linux-2](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/ami) | data source |
| [aws_ami.centos7](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/ami) | data source |
| [aws_ami.centos7-ldap](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/ami) | data source |
| [aws_ami.eks-node](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/ami) | data source |
| [aws_ami.ubuntu](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/ami) | data source |
| [aws_caller_identity.current](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/caller_identity) | data source |
| [aws_iam_policy_document.eks-cluster-autoscaler](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.prometheus](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.vsts-bootstrap-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.vsts-campaign-orchestrator](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.vsts-ci-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.vsts-content-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.vsts-crypto-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.vsts-device-gateway](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.vsts-dim-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.vsts-event-scheduler](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.vsts-gp-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.vsts-kcss-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.vsts-key-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.vsts-notification-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.vsts-proxy-applet-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.vsts-script-executor](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.vsts-sms-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.vsts-statistic-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.vsts-user-service](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iot_endpoint.current](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iot_endpoint) | data source |
| [aws_region.current](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/region) | data source |
| [aws_route53_zone.default](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/route53_zone) | data source |
| [external_external.oidc-thumbprint](https://registry.terraform.io/providers/hashicorp/external/latest/docs/data-sources/external) | data source |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_aws_access_key"></a> [aws\_access\_key](#input\_aws\_access\_key) | Precreated AWS access key. | `string` | `""` | no |
| <a name="input_aws_ecr_region"></a> [aws\_ecr\_region](#input\_aws\_ecr\_region) | AWS ECR region. | `string` | `"us-west-2"` | no |
| <a name="input_aws_region"></a> [aws\_region](#input\_aws\_region) | AWS region. | `string` | `"us-west-2"` | no |
| <a name="input_aws_s3_backup_bucket"></a> [aws\_s3\_backup\_bucket](#input\_aws\_s3\_backup\_bucket) | s3 backup backet name | `string` | `"se-tpm-develop-backup-bucket"` | no |
| <a name="input_aws_secret_key"></a> [aws\_secret\_key](#input\_aws\_secret\_key) | Precreated AWS secret key. | `string` | `""` | no |
| <a name="input_backend_port"></a> [backend\_port](#input\_backend\_port) | The port the service on the EKS instances listen on. | `number` | `31306` | no |
| <a name="input_backend_protocol"></a> [backend\_protocol](#input\_backend\_protocol) | The protocol the EKS cluster. | `string` | `"TCP"` | no |
| <a name="input_bastion_instance_type"></a> [bastion\_instance\_type](#input\_bastion\_instance\_type) | Instance type for Bastion | `string` | `"t3a.micro"` | no |
| <a name="input_branch"></a> [branch](#input\_branch) | Branch from which code was deployed, develop or master. | `string` | `""` | no |
| <a name="input_dns_domain"></a> [dns\_domain](#input\_dns\_domain) | Precreated domain for project in Route53. | `string` | `"se-tpm.com"` | no |
| <a name="input_dns_fullname_wireguard"></a> [dns\_fullname\_wireguard](#input\_dns\_fullname\_wireguard) | Domain name for VPN Wireguard. | `string` | `"wireguard.se-tpm.com"` | no |
| <a name="input_dynamodb_backup"></a> [dynamodb\_backup](#input\_dynamodb\_backup) | Backup retention for dynamodb. | `number` | `7` | no |
| <a name="input_eks_instance_type"></a> [eks\_instance\_type](#input\_eks\_instance\_type) | EKS instance type | `string` | `"t3a.large"` | no |
| <a name="input_eks_node_ami"></a> [eks\_node\_ami](#input\_eks\_node\_ami) | EKS nodes AMI versions map, to fix EKS node version. | `map` | <pre>{<br>  "ap-northeast-1": "ami-022b7082336a35fa5",<br>  "ap-northeast-2": "ami-00e09b556bc0a5250",<br>  "ap-south-1": "ami-02116767eec13d483",<br>  "ap-southeast-1": "ami-0c5b93563fd4c0b64",<br>  "ap-southeast-2": "ami-0fdce91f54abc819c",<br>  "ca-central-1": "ami-07f84ec952ff04c55",<br>  "eu-central-1": "ami-0b63408a8fdf0dfbb",<br>  "eu-north-1": "ami-07852cbef6938d8d4",<br>  "eu-west-1": "ami-072fbef2a16895c26",<br>  "eu-west-3": "ami-063dde54d493f0b10",<br>  "sa-east-1": "ami-0edf89f8165ab8929",<br>  "us-east-1": "ami-09d01d46812c52d7d",<br>  "us-east-2": "ami-0a8371504b52964aa",<br>  "us-west-1": "ami-0d8c692eebb0c2b85",<br>  "us-west-2": "ami-09f3859628fa7c789"<br>}</pre> | no |
| <a name="input_eks_version"></a> [eks\_version](#input\_eks\_version) | EKS version | `string` | `"1.20"` | no |
| <a name="input_elasticsearch_automated_snapshot_start_hour"></a> [elasticsearch\_automated\_snapshot\_start\_hour](#input\_elasticsearch\_automated\_snapshot\_start\_hour) | Elasticsearch automated\_snapshot\_start\_hour | `string` | `"23"` | no |
| <a name="input_elasticsearch_availability_zone_count"></a> [elasticsearch\_availability\_zone\_count](#input\_elasticsearch\_availability\_zone\_count) | Elasticsearch availability zone count | `string` | `"3"` | no |
| <a name="input_elasticsearch_domain_name"></a> [elasticsearch\_domain\_name](#input\_elasticsearch\_domain\_name) | Elasticsearch domain name. | `string` | `"setpm-logs"` | no |
| <a name="input_elasticsearch_ebs_volume_size_apps_logs"></a> [elasticsearch\_ebs\_volume\_size\_apps\_logs](#input\_elasticsearch\_ebs\_volume\_size\_apps\_logs) | Elasticsearch EBS volume size | `string` | `"35"` | no |
| <a name="input_elasticsearch_ebs_volume_size_apps_statistic"></a> [elasticsearch\_ebs\_volume\_size\_apps\_statistic](#input\_elasticsearch\_ebs\_volume\_size\_apps\_statistic) | Elasticsearch EBS volume size | `string` | `"20"` | no |
| <a name="input_elasticsearch_instance_count"></a> [elasticsearch\_instance\_count](#input\_elasticsearch\_instance\_count) | Elasticsearch instance count | `string` | `"3"` | no |
| <a name="input_elasticsearch_instance_type_apps_logs"></a> [elasticsearch\_instance\_type\_apps\_logs](#input\_elasticsearch\_instance\_type\_apps\_logs) | Elasticsearch instance type | `string` | `"t3.medium.elasticsearch"` | no |
| <a name="input_elasticsearch_instance_type_apps_statistic"></a> [elasticsearch\_instance\_type\_apps\_statistic](#input\_elasticsearch\_instance\_type\_apps\_statistic) | Elasticsearch instance type | `string` | `"t3.small.elasticsearch"` | no |
| <a name="input_elasticsearch_version"></a> [elasticsearch\_version](#input\_elasticsearch\_version) | Elasticsearch version | `string` | `"6.8"` | no |
| <a name="input_firebase_token"></a> [firebase\_token](#input\_firebase\_token) | SNS/Platform applications/FCM token for Firebase (FCM) connection. | `string` | `"AAAAKxyqu78:APA91bGnn9-xp7Ev5Yr_T3AuHdlWbjV-a6I7AjhM3tPI_P42sh-V65iP17aPqdQ3rByZZjVpfKUiDOUO5JiMxAmwIezzF2VIGT86nVz_bb7-3xlJzgua2f2o5lhPL4O9Tbcpu_b41Ws1"` | no |
| <a name="input_image_tag"></a> [image\_tag](#input\_image\_tag) | Image tag | `string` | `"develop"` | no |
| <a name="input_iot_se_commands"></a> [iot\_se\_commands](#input\_iot\_se\_commands) | IOT se commands | `string` | `"/v1/se/commands/"` | no |
| <a name="input_iot_se_events"></a> [iot\_se\_events](#input\_iot\_se\_events) | IOT se events | `string` | `"/v1/se/events/"` | no |
| <a name="input_ipsubnet_extaccess"></a> [ipsubnet\_extaccess](#input\_ipsubnet\_extaccess) | External network origins to accept access. | `list` | <pre>[<br>  "195.234.74.0/24",<br>  "195.238.93.0/24",<br>  "195.238.93.128/32",<br>  "34.89.223.156/32",<br>  "83.23.238.209/32",<br>  "46.219.224.0/24",<br>  "95.215.159.102/32",<br>  "92.253.236.242/32",<br>  "176.104.1.114/32",<br>  "188.239.63.103/32",<br>  "89.22.205.90/32",<br>  "24.34.49.120/32",<br>  "71.131.67.132/32",<br>  "109.196.42.90/32"<br>]</pre> | no |
| <a name="input_kubectl_path"></a> [kubectl\_path](#input\_kubectl\_path) | local path to kubectl binary. | `string` | `""` | no |
| <a name="input_mail_sender_address"></a> [mail\_sender\_address](#input\_mail\_sender\_address) | Email sender address. Note: should be manually varified in AWS SES service. | `string` | `"tsm.portal.lite@gmail.com"` | no |
| <a name="input_openldap_admin_user"></a> [openldap\_admin\_user](#input\_openldap\_admin\_user) | Administrator user for OpenLDAP. | `string` | `"admin"` | no |
| <a name="input_openldap_instance_type"></a> [openldap\_instance\_type](#input\_openldap\_instance\_type) | openldap instance type | `string` | `"t3a.micro"` | no |
| <a name="input_ssh_key"></a> [ssh\_key](#input\_ssh\_key) | SSH-key for EC2. | `string` | `"globallogic-tpm"` | no |
| <a name="input_tags"></a> [tags](#input\_tags) | Default tags set. | `map` | <pre>{<br>  "Creator": "GL-DevOpsTeam",<br>  "Environment": "develop",<br>  "Project": "SETPM",<br>  "Release": "1.0"<br>}</pre> | no |
| <a name="input_target_type"></a> [target\_type](#input\_target\_type) | The type of target | `string` | `"instance"` | no |
| <a name="input_vpc_cidr_starting_ip"></a> [vpc\_cidr\_starting\_ip](#input\_vpc\_cidr\_starting\_ip) | This value will serve as the starting IP for a /16 CIDR. Example: a value of 10.0.0.0 will result in CIDR 10.0.0.0/16. | `string` | `"101.101.0.0"` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_AWS_CERT_BUCKET_NAME"></a> [AWS\_CERT\_BUCKET\_NAME](#output\_AWS\_CERT\_BUCKET\_NAME) | n/a |
| <a name="output_DYNAMO_APIKEY_CS_TABLE"></a> [DYNAMO\_APIKEY\_CS\_TABLE](#output\_DYNAMO\_APIKEY\_CS\_TABLE) | n/a |
| <a name="output_DYNAMO_APIKEY_DG_TABLE"></a> [DYNAMO\_APIKEY\_DG\_TABLE](#output\_DYNAMO\_APIKEY\_DG\_TABLE) | n/a |
| <a name="output_DYNAMO_APIKEY_TABLE"></a> [DYNAMO\_APIKEY\_TABLE](#output\_DYNAMO\_APIKEY\_TABLE) | vsts-user-service |
| <a name="output_DYNAMO_APPLET_TABLE"></a> [DYNAMO\_APPLET\_TABLE](#output\_DYNAMO\_APPLET\_TABLE) | n/a |
| <a name="output_DYNAMO_BS_ICCID_INFO_TABLE"></a> [DYNAMO\_BS\_ICCID\_INFO\_TABLE](#output\_DYNAMO\_BS\_ICCID\_INFO\_TABLE) | n/a |
| <a name="output_DYNAMO_CAMPAIGN_EXECUTION_TABLE_CAMPAIGN_ORCHESTARTOR"></a> [DYNAMO\_CAMPAIGN\_EXECUTION\_TABLE\_CAMPAIGN\_ORCHESTARTOR](#output\_DYNAMO\_CAMPAIGN\_EXECUTION\_TABLE\_CAMPAIGN\_ORCHESTARTOR) | n/a |
| <a name="output_DYNAMO_CAMPAIGN_EXECUTION_TABLE_CONTENT_SERVICE"></a> [DYNAMO\_CAMPAIGN\_EXECUTION\_TABLE\_CONTENT\_SERVICE](#output\_DYNAMO\_CAMPAIGN\_EXECUTION\_TABLE\_CONTENT\_SERVICE) | n/a |
| <a name="output_DYNAMO_CAMPAIGN_TABLE"></a> [DYNAMO\_CAMPAIGN\_TABLE](#output\_DYNAMO\_CAMPAIGN\_TABLE) | n/a |
| <a name="output_DYNAMO_COMMAND_EXECUTION_TABLE"></a> [DYNAMO\_COMMAND\_EXECUTION\_TABLE](#output\_DYNAMO\_COMMAND\_EXECUTION\_TABLE) | n/a |
| <a name="output_DYNAMO_COMMAND_PREPARATION_TABLE"></a> [DYNAMO\_COMMAND\_PREPARATION\_TABLE](#output\_DYNAMO\_COMMAND\_PREPARATION\_TABLE) | n/a |
| <a name="output_DYNAMO_COMMAND_PREPARATION_TABLE_GP"></a> [DYNAMO\_COMMAND\_PREPARATION\_TABLE\_GP](#output\_DYNAMO\_COMMAND\_PREPARATION\_TABLE\_GP) | n/a |
| <a name="output_DYNAMO_CS_SCRIPT_EXECUTION"></a> [DYNAMO\_CS\_SCRIPT\_EXECUTION](#output\_DYNAMO\_CS\_SCRIPT\_EXECUTION) | vsts-lambda-db-campaign-execution |
| <a name="output_DYNAMO_CUSTOM_COMMANDS_TABLE"></a> [DYNAMO\_CUSTOM\_COMMANDS\_TABLE](#output\_DYNAMO\_CUSTOM\_COMMANDS\_TABLE) | n/a |
| <a name="output_DYNAMO_DEVICE_COMMAND_TABLE"></a> [DYNAMO\_DEVICE\_COMMAND\_TABLE](#output\_DYNAMO\_DEVICE\_COMMAND\_TABLE) | n/a |
| <a name="output_DYNAMO_DEVICE_CONFIG_LINKS"></a> [DYNAMO\_DEVICE\_CONFIG\_LINKS](#output\_DYNAMO\_DEVICE\_CONFIG\_LINKS) | n/a |
| <a name="output_DYNAMO_DEVICE_INFO_TABLE"></a> [DYNAMO\_DEVICE\_INFO\_TABLE](#output\_DYNAMO\_DEVICE\_INFO\_TABLE) | n/a |
| <a name="output_DYNAMO_DEVICE_NOTIFICATIONS_TABLE"></a> [DYNAMO\_DEVICE\_NOTIFICATIONS\_TABLE](#output\_DYNAMO\_DEVICE\_NOTIFICATIONS\_TABLE) | n/a |
| <a name="output_DYNAMO_DG_VENDOR_TABLE"></a> [DYNAMO\_DG\_VENDOR\_TABLE](#output\_DYNAMO\_DG\_VENDOR\_TABLE) | n/a |
| <a name="output_DYNAMO_GROUPED_COMMANDS_TABLE"></a> [DYNAMO\_GROUPED\_COMMANDS\_TABLE](#output\_DYNAMO\_GROUPED\_COMMANDS\_TABLE) | n/a |
| <a name="output_DYNAMO_ICCID_RELATIONS_TABLE_SK_PK_INDEX"></a> [DYNAMO\_ICCID\_RELATIONS\_TABLE\_SK\_PK\_INDEX](#output\_DYNAMO\_ICCID\_RELATIONS\_TABLE\_SK\_PK\_INDEX) | n/a |
| <a name="output_DYNAMO_KS_ICCID_INFO"></a> [DYNAMO\_KS\_ICCID\_INFO](#output\_DYNAMO\_KS\_ICCID\_INFO) | n/a |
| <a name="output_DYNAMO_RELATION_PROFILE_TABLE"></a> [DYNAMO\_RELATION\_PROFILE\_TABLE](#output\_DYNAMO\_RELATION\_PROFILE\_TABLE) | n/a |
| <a name="output_DYNAMO_RELATION_PROFILE_TABLE_NAME_SCRIPT_ID_INDEX"></a> [DYNAMO\_RELATION\_PROFILE\_TABLE\_NAME\_SCRIPT\_ID\_INDEX](#output\_DYNAMO\_RELATION\_PROFILE\_TABLE\_NAME\_SCRIPT\_ID\_INDEX) | n/a |
| <a name="output_DYNAMO_ROLE_TABLE"></a> [DYNAMO\_ROLE\_TABLE](#output\_DYNAMO\_ROLE\_TABLE) | n/a |
| <a name="output_DYNAMO_SCHEDULED_EVENT_TABLE"></a> [DYNAMO\_SCHEDULED\_EVENT\_TABLE](#output\_DYNAMO\_SCHEDULED\_EVENT\_TABLE) | vsts-event-scheduler |
| <a name="output_DYNAMO_SCRIPT_EXECUTION_TABLE_CAMPAIGN_ORCHESTRATOR"></a> [DYNAMO\_SCRIPT\_EXECUTION\_TABLE\_CAMPAIGN\_ORCHESTRATOR](#output\_DYNAMO\_SCRIPT\_EXECUTION\_TABLE\_CAMPAIGN\_ORCHESTRATOR) | vsts-campaign-orchestrator |
| <a name="output_DYNAMO_SCRIPT_EXECUTION_TABLE_CONTENT_SERVICE"></a> [DYNAMO\_SCRIPT\_EXECUTION\_TABLE\_CONTENT\_SERVICE](#output\_DYNAMO\_SCRIPT\_EXECUTION\_TABLE\_CONTENT\_SERVICE) | n/a |
| <a name="output_DYNAMO_SCRIPT_TABLE"></a> [DYNAMO\_SCRIPT\_TABLE](#output\_DYNAMO\_SCRIPT\_TABLE) | n/a |
| <a name="output_DYNAMO_SCRIPT_TABLE_SRV_SCRIPT_EXECUTOR"></a> [DYNAMO\_SCRIPT\_TABLE\_SRV\_SCRIPT\_EXECUTOR](#output\_DYNAMO\_SCRIPT\_TABLE\_SRV\_SCRIPT\_EXECUTOR) | n/a |
| <a name="output_DYNAMO_SCRIPT_TEMPLATE_TABLE"></a> [DYNAMO\_SCRIPT\_TEMPLATE\_TABLE](#output\_DYNAMO\_SCRIPT\_TEMPLATE\_TABLE) | n/a |
| <a name="output_DYNAMO_SCRIPT_TEMPLATE_TABLE_NAME_VENDOR_ID_INDEX"></a> [DYNAMO\_SCRIPT\_TEMPLATE\_TABLE\_NAME\_VENDOR\_ID\_INDEX](#output\_DYNAMO\_SCRIPT\_TEMPLATE\_TABLE\_NAME\_VENDOR\_ID\_INDEX) | n/a |
| <a name="output_DYNAMO_SUPPORTED_CA_TABLE"></a> [DYNAMO\_SUPPORTED\_CA\_TABLE](#output\_DYNAMO\_SUPPORTED\_CA\_TABLE) | n/a |
| <a name="output_DYNAMO_SUPPORTED_COMMANDS_TABLE"></a> [DYNAMO\_SUPPORTED\_COMMANDS\_TABLE](#output\_DYNAMO\_SUPPORTED\_COMMANDS\_TABLE) | n/a |
| <a name="output_DYNAMO_TABLE_GP_APPLET"></a> [DYNAMO\_TABLE\_GP\_APPLET](#output\_DYNAMO\_TABLE\_GP\_APPLET) | n/a |
| <a name="output_DYNAMO_TABLE_ICCID"></a> [DYNAMO\_TABLE\_ICCID](#output\_DYNAMO\_TABLE\_ICCID) | n/a |
| <a name="output_DYNAMO_TABLE_IDENTITIES"></a> [DYNAMO\_TABLE\_IDENTITIES](#output\_DYNAMO\_TABLE\_IDENTITIES) | n/a |
| <a name="output_DYNAMO_UICC_GROUP_TABLE"></a> [DYNAMO\_UICC\_GROUP\_TABLE](#output\_DYNAMO\_UICC\_GROUP\_TABLE) | n/a |
| <a name="output_DYNAMO_UICC_STATUS_INDEX_NAME"></a> [DYNAMO\_UICC\_STATUS\_INDEX\_NAME](#output\_DYNAMO\_UICC\_STATUS\_INDEX\_NAME) | n/a |
| <a name="output_DYNAMO_UICC_TABLE"></a> [DYNAMO\_UICC\_TABLE](#output\_DYNAMO\_UICC\_TABLE) | n/a |
| <a name="output_DYNAMO_USER_INFO_TABLE"></a> [DYNAMO\_USER\_INFO\_TABLE](#output\_DYNAMO\_USER\_INFO\_TABLE) | n/a |
| <a name="output_DYNAMO_USER_TABLE"></a> [DYNAMO\_USER\_TABLE](#output\_DYNAMO\_USER\_TABLE) | n/a |
| <a name="output_DYNAMO_VENDOR_INFO_TABLE"></a> [DYNAMO\_VENDOR\_INFO\_TABLE](#output\_DYNAMO\_VENDOR\_INFO\_TABLE) | n/a |
| <a name="output_DYNAMO_VENDOR_PERMISSIONS_TABLE"></a> [DYNAMO\_VENDOR\_PERMISSIONS\_TABLE](#output\_DYNAMO\_VENDOR\_PERMISSIONS\_TABLE) | n/a |
| <a name="output_DYNAMO_VENDOR_TABLE"></a> [DYNAMO\_VENDOR\_TABLE](#output\_DYNAMO\_VENDOR\_TABLE) | n/a |
| <a name="output_IOT_BROKER_URL"></a> [IOT\_BROKER\_URL](#output\_IOT\_BROKER\_URL) | n/a |
| <a name="output_PROXY_APPLET_COMMAND_TABLE"></a> [PROXY\_APPLET\_COMMAND\_TABLE](#output\_PROXY\_APPLET\_COMMAND\_TABLE) | n/a |
| <a name="output_PROXY_APPLET_COMMAND_TABLE_INDEX"></a> [PROXY\_APPLET\_COMMAND\_TABLE\_INDEX](#output\_PROXY\_APPLET\_COMMAND\_TABLE\_INDEX) | n/a |
| <a name="output_PROXY_APPLET_SESSION_INFO"></a> [PROXY\_APPLET\_SESSION\_INFO](#output\_PROXY\_APPLET\_SESSION\_INFO) | n/a |
| <a name="output_SE_DEVICE_INFO_QUEUE"></a> [SE\_DEVICE\_INFO\_QUEUE](#output\_SE\_DEVICE\_INFO\_QUEUE) | n/a |
| <a name="output_SE_DEVICE_INFO_TABLE"></a> [SE\_DEVICE\_INFO\_TABLE](#output\_SE\_DEVICE\_INFO\_TABLE) | n/a |
| <a name="output_SNS_CA_CERT_GEN_TOPIC"></a> [SNS\_CA\_CERT\_GEN\_TOPIC](#output\_SNS\_CA\_CERT\_GEN\_TOPIC) | n/a |
| <a name="output_SNS_CA_COMMANDS"></a> [SNS\_CA\_COMMANDS](#output\_SNS\_CA\_COMMANDS) | n/a |
| <a name="output_SNS_CA_EVENTS_TOPIC"></a> [SNS\_CA\_EVENTS\_TOPIC](#output\_SNS\_CA\_EVENTS\_TOPIC) | n/a |
| <a name="output_SNS_CHANNEL_APPLET_EVENTS"></a> [SNS\_CHANNEL\_APPLET\_EVENTS](#output\_SNS\_CHANNEL\_APPLET\_EVENTS) | n/a |
| <a name="output_SNS_CHANNEL_BOOTSTRAP_EVENTS"></a> [SNS\_CHANNEL\_BOOTSTRAP\_EVENTS](#output\_SNS\_CHANNEL\_BOOTSTRAP\_EVENTS) | vsts-bootstrap-service |
| <a name="output_SNS_CHANNEL_CAMPAIGN_COMMANDS"></a> [SNS\_CHANNEL\_CAMPAIGN\_COMMANDS](#output\_SNS\_CHANNEL\_CAMPAIGN\_COMMANDS) | vsts-content-service |
| <a name="output_SNS_CHANNEL_CAMPAIGN_EVENTS"></a> [SNS\_CHANNEL\_CAMPAIGN\_EVENTS](#output\_SNS\_CHANNEL\_CAMPAIGN\_EVENTS) | n/a |
| <a name="output_SNS_CHANNEL_CAMPAIGN_EVENTS_ARN"></a> [SNS\_CHANNEL\_CAMPAIGN\_EVENTS\_ARN](#output\_SNS\_CHANNEL\_CAMPAIGN\_EVENTS\_ARN) | n/a |
| <a name="output_SNS_CHANNEL_CRYPTO_EVENTS"></a> [SNS\_CHANNEL\_CRYPTO\_EVENTS](#output\_SNS\_CHANNEL\_CRYPTO\_EVENTS) | n/a |
| <a name="output_SNS_CHANNEL_CRYPTO_SERVICE_EVENTS"></a> [SNS\_CHANNEL\_CRYPTO\_SERVICE\_EVENTS](#output\_SNS\_CHANNEL\_CRYPTO\_SERVICE\_EVENTS) | n/a |
| <a name="output_SNS_CHANNEL_DEVICE_NOTIFICATIONS"></a> [SNS\_CHANNEL\_DEVICE\_NOTIFICATIONS](#output\_SNS\_CHANNEL\_DEVICE\_NOTIFICATIONS) | vsts-notification-service |
| <a name="output_SNS_CHANNEL_GP_CRYPTO_EVENTS"></a> [SNS\_CHANNEL\_GP\_CRYPTO\_EVENTS](#output\_SNS\_CHANNEL\_GP\_CRYPTO\_EVENTS) | n/a |
| <a name="output_SNS_CHANNEL_PROXY_APPLET_DEVICE_COMMANDS"></a> [SNS\_CHANNEL\_PROXY\_APPLET\_DEVICE\_COMMANDS](#output\_SNS\_CHANNEL\_PROXY\_APPLET\_DEVICE\_COMMANDS) | vsts-proxy-applet-service |
| <a name="output_SNS_CHANNEL_SCHEDULED_EVENTS"></a> [SNS\_CHANNEL\_SCHEDULED\_EVENTS](#output\_SNS\_CHANNEL\_SCHEDULED\_EVENTS) | n/a |
| <a name="output_SNS_CHANNEL_SCRIPT_COMMANDS"></a> [SNS\_CHANNEL\_SCRIPT\_COMMANDS](#output\_SNS\_CHANNEL\_SCRIPT\_COMMANDS) | n/a |
| <a name="output_SNS_CHANNEL_STATISTIC_TOPIC"></a> [SNS\_CHANNEL\_STATISTIC\_TOPIC](#output\_SNS\_CHANNEL\_STATISTIC\_TOPIC) | n/a |
| <a name="output_SNS_CHANNEL_USER_COMMANDS"></a> [SNS\_CHANNEL\_USER\_COMMANDS](#output\_SNS\_CHANNEL\_USER\_COMMANDS) | n/a |
| <a name="output_SNS_CHANNEL_USER_EVENTS"></a> [SNS\_CHANNEL\_USER\_EVENTS](#output\_SNS\_CHANNEL\_USER\_EVENTS) | n/a |
| <a name="output_SNS_CI_COMMANDS_TOPIC"></a> [SNS\_CI\_COMMANDS\_TOPIC](#output\_SNS\_CI\_COMMANDS\_TOPIC) | n/a |
| <a name="output_SNS_CI_EVENTS_TOPIC"></a> [SNS\_CI\_EVENTS\_TOPIC](#output\_SNS\_CI\_EVENTS\_TOPIC) | vsts-ci-service |
| <a name="output_SNS_COMMAND_EVENTS_TOPIC"></a> [SNS\_COMMAND\_EVENTS\_TOPIC](#output\_SNS\_COMMAND\_EVENTS\_TOPIC) | n/a |
| <a name="output_SNS_CRYPTO_COMMANDS_TOPIC"></a> [SNS\_CRYPTO\_COMMANDS\_TOPIC](#output\_SNS\_CRYPTO\_COMMANDS\_TOPIC) | n/a |
| <a name="output_SNS_DEVICE_COMMANDS_TOPIC"></a> [SNS\_DEVICE\_COMMANDS\_TOPIC](#output\_SNS\_DEVICE\_COMMANDS\_TOPIC) | n/a |
| <a name="output_SNS_DEVICE_EVENTS_TOPIC"></a> [SNS\_DEVICE\_EVENTS\_TOPIC](#output\_SNS\_DEVICE\_EVENTS\_TOPIC) | vsts-device-gateway |
| <a name="output_SNS_DEVICE_INFO_TOPIC"></a> [SNS\_DEVICE\_INFO\_TOPIC](#output\_SNS\_DEVICE\_INFO\_TOPIC) | n/a |
| <a name="output_SNS_GP_CI_EVENTS_TOPIC"></a> [SNS\_GP\_CI\_EVENTS\_TOPIC](#output\_SNS\_GP\_CI\_EVENTS\_TOPIC) | n/a |
| <a name="output_SNS_GP_COMMANDS_TOPIC"></a> [SNS\_GP\_COMMANDS\_TOPIC](#output\_SNS\_GP\_COMMANDS\_TOPIC) | n/a |
| <a name="output_SNS_KCSS_COMMANDS_TOPIC"></a> [SNS\_KCSS\_COMMANDS\_TOPIC](#output\_SNS\_KCSS\_COMMANDS\_TOPIC) | n/a |
| <a name="output_SNS_KEYS_COMMANDS"></a> [SNS\_KEYS\_COMMANDS](#output\_SNS\_KEYS\_COMMANDS) | n/a |
| <a name="output_SNS_KEYS_EVENTS"></a> [SNS\_KEYS\_EVENTS](#output\_SNS\_KEYS\_EVENTS) | n/a |
| <a name="output_SNS_KEY_SERVICE_COMMANDS"></a> [SNS\_KEY\_SERVICE\_COMMANDS](#output\_SNS\_KEY\_SERVICE\_COMMANDS) | n/a |
| <a name="output_SNS_PROXY_APPLET_COMMANDS"></a> [SNS\_PROXY\_APPLET\_COMMANDS](#output\_SNS\_PROXY\_APPLET\_COMMANDS) | n/a |
| <a name="output_SNS_PUSH_NOTIFICATION_ARN"></a> [SNS\_PUSH\_NOTIFICATION\_ARN](#output\_SNS\_PUSH\_NOTIFICATION\_ARN) | n/a |
| <a name="output_SNS_SCRIPT_COMMANDS_SUPPORTED_TOPIC"></a> [SNS\_SCRIPT\_COMMANDS\_SUPPORTED\_TOPIC](#output\_SNS\_SCRIPT\_COMMANDS\_SUPPORTED\_TOPIC) | n/a |
| <a name="output_SNS_SCRIPT_EVENTS_TOPIC"></a> [SNS\_SCRIPT\_EVENTS\_TOPIC](#output\_SNS\_SCRIPT\_EVENTS\_TOPIC) | n/a |
| <a name="output_SNS_STATISTICS_EVENTS"></a> [SNS\_STATISTICS\_EVENTS](#output\_SNS\_STATISTICS\_EVENTS) | n/a |
| <a name="output_SNS_SUPPORTED_COMMANDS_TOPIC"></a> [SNS\_SUPPORTED\_COMMANDS\_TOPIC](#output\_SNS\_SUPPORTED\_COMMANDS\_TOPIC) | vsts-kcss-service |
| <a name="output_SNS_TOPIC_PREFIX"></a> [SNS\_TOPIC\_PREFIX](#output\_SNS\_TOPIC\_PREFIX) | n/a |
| <a name="output_SNS_UICC"></a> [SNS\_UICC](#output\_SNS\_UICC) | n/a |
| <a name="output_SQS_CA_CERT_GEN_QUEUE"></a> [SQS\_CA\_CERT\_GEN\_QUEUE](#output\_SQS\_CA\_CERT\_GEN\_QUEUE) | n/a |
| <a name="output_SQS_CA_COMMANDS"></a> [SQS\_CA\_COMMANDS](#output\_SQS\_CA\_COMMANDS) | n/a |
| <a name="output_SQS_CHANNEL_APPLET_EVENTS"></a> [SQS\_CHANNEL\_APPLET\_EVENTS](#output\_SQS\_CHANNEL\_APPLET\_EVENTS) | n/a |
| <a name="output_SQS_CHANNEL_BOOTSTRAP_EVENTS"></a> [SQS\_CHANNEL\_BOOTSTRAP\_EVENTS](#output\_SQS\_CHANNEL\_BOOTSTRAP\_EVENTS) | n/a |
| <a name="output_SQS_CHANNEL_CAMPAIGN_COMMANDS"></a> [SQS\_CHANNEL\_CAMPAIGN\_COMMANDS](#output\_SQS\_CHANNEL\_CAMPAIGN\_COMMANDS) | n/a |
| <a name="output_SQS_CHANNEL_CAMPAIGN_EVENTS"></a> [SQS\_CHANNEL\_CAMPAIGN\_EVENTS](#output\_SQS\_CHANNEL\_CAMPAIGN\_EVENTS) | n/a |
| <a name="output_SQS_CHANNEL_CA_EVENTS"></a> [SQS\_CHANNEL\_CA\_EVENTS](#output\_SQS\_CHANNEL\_CA\_EVENTS) | n/a |
| <a name="output_SQS_CHANNEL_CRYPTO_COMMANDS"></a> [SQS\_CHANNEL\_CRYPTO\_COMMANDS](#output\_SQS\_CHANNEL\_CRYPTO\_COMMANDS) | vsts-crypto-service |
| <a name="output_SQS_CHANNEL_DEVICE_NOTIFICATIONS"></a> [SQS\_CHANNEL\_DEVICE\_NOTIFICATIONS](#output\_SQS\_CHANNEL\_DEVICE\_NOTIFICATIONS) | n/a |
| <a name="output_SQS_CHANNEL_GENERIC_EVENTS"></a> [SQS\_CHANNEL\_GENERIC\_EVENTS](#output\_SQS\_CHANNEL\_GENERIC\_EVENTS) | n/a |
| <a name="output_SQS_CHANNEL_GP_CRYPTO_EVENTS"></a> [SQS\_CHANNEL\_GP\_CRYPTO\_EVENTS](#output\_SQS\_CHANNEL\_GP\_CRYPTO\_EVENTS) | n/a |
| <a name="output_SQS_CHANNEL_ICCID_EVENTS"></a> [SQS\_CHANNEL\_ICCID\_EVENTS](#output\_SQS\_CHANNEL\_ICCID\_EVENTS) | n/a |
| <a name="output_SQS_CHANNEL_KS_UICC"></a> [SQS\_CHANNEL\_KS\_UICC](#output\_SQS\_CHANNEL\_KS\_UICC) | n/a |
| <a name="output_SQS_CHANNEL_PROXY_APPLET_DEVICE_COMMAND_EVENTS"></a> [SQS\_CHANNEL\_PROXY\_APPLET\_DEVICE\_COMMAND\_EVENTS](#output\_SQS\_CHANNEL\_PROXY\_APPLET\_DEVICE\_COMMAND\_EVENTS) | n/a |
| <a name="output_SQS_CHANNEL_SCHEDULED_EVENTS_COMMANDS"></a> [SQS\_CHANNEL\_SCHEDULED\_EVENTS\_COMMANDS](#output\_SQS\_CHANNEL\_SCHEDULED\_EVENTS\_COMMANDS) | n/a |
| <a name="output_SQS_CHANNEL_SCRIPT_EVENTS"></a> [SQS\_CHANNEL\_SCRIPT\_EVENTS](#output\_SQS\_CHANNEL\_SCRIPT\_EVENTS) | n/a |
| <a name="output_SQS_CHANNEL_SECURE_MESSAGING_EVENTS"></a> [SQS\_CHANNEL\_SECURE\_MESSAGING\_EVENTS](#output\_SQS\_CHANNEL\_SECURE\_MESSAGING\_EVENTS) | n/a |
| <a name="output_SQS_CHANNEL_STATISTIC_QUEUE"></a> [SQS\_CHANNEL\_STATISTIC\_QUEUE](#output\_SQS\_CHANNEL\_STATISTIC\_QUEUE) | vsts-statistic-service |
| <a name="output_SQS_CHANNEL_SUPPORTED_COMMANDS_EVENTS"></a> [SQS\_CHANNEL\_SUPPORTED\_COMMANDS\_EVENTS](#output\_SQS\_CHANNEL\_SUPPORTED\_COMMANDS\_EVENTS) | n/a |
| <a name="output_SQS_CHANNEL_USER_COMMANDS"></a> [SQS\_CHANNEL\_USER\_COMMANDS](#output\_SQS\_CHANNEL\_USER\_COMMANDS) | n/a |
| <a name="output_SQS_CHANNEL_USER_EVENTS"></a> [SQS\_CHANNEL\_USER\_EVENTS](#output\_SQS\_CHANNEL\_USER\_EVENTS) | n/a |
| <a name="output_SQS_CHANNEL_VENDOR_CO_EVENTS"></a> [SQS\_CHANNEL\_VENDOR\_CO\_EVENTS](#output\_SQS\_CHANNEL\_VENDOR\_CO\_EVENTS) | n/a |
| <a name="output_SQS_CHANNEL_VENDOR_EVENTS"></a> [SQS\_CHANNEL\_VENDOR\_EVENTS](#output\_SQS\_CHANNEL\_VENDOR\_EVENTS) | n/a |
| <a name="output_SQS_CI_COMMANDS_QUEUE"></a> [SQS\_CI\_COMMANDS\_QUEUE](#output\_SQS\_CI\_COMMANDS\_QUEUE) | n/a |
| <a name="output_SQS_CI_EVENTS_QUEUE"></a> [SQS\_CI\_EVENTS\_QUEUE](#output\_SQS\_CI\_EVENTS\_QUEUE) | common with script-executor-service |
| <a name="output_SQS_COMMAND_EVENTS_QUEUE"></a> [SQS\_COMMAND\_EVENTS\_QUEUE](#output\_SQS\_COMMAND\_EVENTS\_QUEUE) | n/a |
| <a name="output_SQS_CRYPTO_EVENTS_QUEUE"></a> [SQS\_CRYPTO\_EVENTS\_QUEUE](#output\_SQS\_CRYPTO\_EVENTS\_QUEUE) | n/a |
| <a name="output_SQS_DEVICE_COMMANDS_QUEUE"></a> [SQS\_DEVICE\_COMMANDS\_QUEUE](#output\_SQS\_DEVICE\_COMMANDS\_QUEUE) | n/a |
| <a name="output_SQS_DEVICE_EVENTS_QUEUE"></a> [SQS\_DEVICE\_EVENTS\_QUEUE](#output\_SQS\_DEVICE\_EVENTS\_QUEUE) | n/a |
| <a name="output_SQS_DEVICE_INFO_EVENTS"></a> [SQS\_DEVICE\_INFO\_EVENTS](#output\_SQS\_DEVICE\_INFO\_EVENTS) | n/a |
| <a name="output_SQS_DEVICE_ONBOARD_QUEUE"></a> [SQS\_DEVICE\_ONBOARD\_QUEUE](#output\_SQS\_DEVICE\_ONBOARD\_QUEUE) | n/a |
| <a name="output_SQS_DIM_COMMAND_EVENTS_QUEUE"></a> [SQS\_DIM\_COMMAND\_EVENTS\_QUEUE](#output\_SQS\_DIM\_COMMAND\_EVENTS\_QUEUE) | n/a |
| <a name="output_SQS_DIM_DEVICE_EVENTS_QUEUE"></a> [SQS\_DIM\_DEVICE\_EVENTS\_QUEUE](#output\_SQS\_DIM\_DEVICE\_EVENTS\_QUEUE) | n/a |
| <a name="output_SQS_GP_CI_EVENTS_QUEUE"></a> [SQS\_GP\_CI\_EVENTS\_QUEUE](#output\_SQS\_GP\_CI\_EVENTS\_QUEUE) | n/a |
| <a name="output_SQS_GP_COMMANDS_QUEUE"></a> [SQS\_GP\_COMMANDS\_QUEUE](#output\_SQS\_GP\_COMMANDS\_QUEUE) | n/a |
| <a name="output_SQS_KCSS_COMMANDS_QUEUE"></a> [SQS\_KCSS\_COMMANDS\_QUEUE](#output\_SQS\_KCSS\_COMMANDS\_QUEUE) | n/a |
| <a name="output_SQS_KEYS_COMMANDS"></a> [SQS\_KEYS\_COMMANDS](#output\_SQS\_KEYS\_COMMANDS) | n/a |
| <a name="output_SQS_KEYS_EVENTS"></a> [SQS\_KEYS\_EVENTS](#output\_SQS\_KEYS\_EVENTS) | n/a |
| <a name="output_SQS_KEY_SERVICE_EVENTS"></a> [SQS\_KEY\_SERVICE\_EVENTS](#output\_SQS\_KEY\_SERVICE\_EVENTS) | n/a |
| <a name="output_SQS_QUEUE_PREFIX"></a> [SQS\_QUEUE\_PREFIX](#output\_SQS\_QUEUE\_PREFIX) | n/a |
| <a name="output_SQS_SCRIPT_COMMANDS_QUEUE"></a> [SQS\_SCRIPT\_COMMANDS\_QUEUE](#output\_SQS\_SCRIPT\_COMMANDS\_QUEUE) | vsts-script-executor |
| <a name="output_SQS_SE_EVENTS_QUEUE"></a> [SQS\_SE\_EVENTS\_QUEUE](#output\_SQS\_SE\_EVENTS\_QUEUE) | n/a |
| <a name="output_SQS_UICC"></a> [SQS\_UICC](#output\_SQS\_UICC) | n/a |
| <a name="output_SQS_USER_COMMANDS_QUEUE"></a> [SQS\_USER\_COMMANDS\_QUEUE](#output\_SQS\_USER\_COMMANDS\_QUEUE) | n/a |
| <a name="output_SQS_VENDOR_EVENTS_QUEUE"></a> [SQS\_VENDOR\_EVENTS\_QUEUE](#output\_SQS\_VENDOR\_EVENTS\_QUEUE) | n/a |
| <a name="output_api_gateway_domain_name"></a> [api\_gateway\_domain\_name](#output\_api\_gateway\_domain\_name) | n/a |
| <a name="output_aws_account_id"></a> [aws\_account\_id](#output\_aws\_account\_id) | n/a |
| <a name="output_aws_acm_certificate_arn"></a> [aws\_acm\_certificate\_arn](#output\_aws\_acm\_certificate\_arn) | n/a |
| <a name="output_aws_campaign_bucket_name"></a> [aws\_campaign\_bucket\_name](#output\_aws\_campaign\_bucket\_name) | n/a |
| <a name="output_aws_ecr_region"></a> [aws\_ecr\_region](#output\_aws\_ecr\_region) | n/a |
| <a name="output_aws_iot_certificate_cert_thing_backend_client_certificate_pem"></a> [aws\_iot\_certificate\_cert\_thing\_backend\_client\_certificate\_pem](#output\_aws\_iot\_certificate\_cert\_thing\_backend\_client\_certificate\_pem) | n/a |
| <a name="output_aws_iot_certificate_cert_thing_backend_client_private_key"></a> [aws\_iot\_certificate\_cert\_thing\_backend\_client\_private\_key](#output\_aws\_iot\_certificate\_cert\_thing\_backend\_client\_private\_key) | n/a |
| <a name="output_aws_region"></a> [aws\_region](#output\_aws\_region) | n/a |
| <a name="output_aws_s3_backup_bucket"></a> [aws\_s3\_backup\_bucket](#output\_aws\_s3\_backup\_bucket) | n/a |
| <a name="output_ca_certificates"></a> [ca\_certificates](#output\_ca\_certificates) | n/a |
| <a name="output_dns_domain"></a> [dns\_domain](#output\_dns\_domain) | n/a |
| <a name="output_dns_fullname"></a> [dns\_fullname](#output\_dns\_fullname) | n/a |
| <a name="output_dns_fullname_frontend"></a> [dns\_fullname\_frontend](#output\_dns\_fullname\_frontend) | n/a |
| <a name="output_efs_key_service_dns_name"></a> [efs\_key\_service\_dns\_name](#output\_efs\_key\_service\_dns\_name) | n/a |
| <a name="output_efs_key_service_id"></a> [efs\_key\_service\_id](#output\_efs\_key\_service\_id) | n/a |
| <a name="output_eks_cluster_endpoint"></a> [eks\_cluster\_endpoint](#output\_eks\_cluster\_endpoint) | n/a |
| <a name="output_eks_cluster_name"></a> [eks\_cluster\_name](#output\_eks\_cluster\_name) | n/a |
| <a name="output_eks_instance_role_arn"></a> [eks\_instance\_role\_arn](#output\_eks\_instance\_role\_arn) | n/a |
| <a name="output_elasticsearch_endpoint"></a> [elasticsearch\_endpoint](#output\_elasticsearch\_endpoint) | n/a |
| <a name="output_elasticsearch_endpoint_statistic"></a> [elasticsearch\_endpoint\_statistic](#output\_elasticsearch\_endpoint\_statistic) | n/a |
| <a name="output_iam_mail_sender_user_aws_access_key"></a> [iam\_mail\_sender\_user\_aws\_access\_key](#output\_iam\_mail\_sender\_user\_aws\_access\_key) | n/a |
| <a name="output_iam_mail_sender_user_aws_secret_key"></a> [iam\_mail\_sender\_user\_aws\_secret\_key](#output\_iam\_mail\_sender\_user\_aws\_secret\_key) | n/a |
| <a name="output_image_tag"></a> [image\_tag](#output\_image\_tag) | n/a |
| <a name="output_iot_se_commands"></a> [iot\_se\_commands](#output\_iot\_se\_commands) | n/a |
| <a name="output_iot_se_events"></a> [iot\_se\_events](#output\_iot\_se\_events) | n/a |
| <a name="output_kub_eks_cluster_autoscaler"></a> [kub\_eks\_cluster\_autoscaler](#output\_kub\_eks\_cluster\_autoscaler) | n/a |
| <a name="output_kub_lambda-api-gateway_role_arn"></a> [kub\_lambda-api-gateway\_role\_arn](#output\_kub\_lambda-api-gateway\_role\_arn) | n/a |
| <a name="output_kub_prometheus_role_arn"></a> [kub\_prometheus\_role\_arn](#output\_kub\_prometheus\_role\_arn) | n/a |
| <a name="output_kub_vsts_bootstrap_service_role_arn"></a> [kub\_vsts\_bootstrap\_service\_role\_arn](#output\_kub\_vsts\_bootstrap\_service\_role\_arn) | n/a |
| <a name="output_kub_vsts_campaign_orchestrator_role_arn"></a> [kub\_vsts\_campaign\_orchestrator\_role\_arn](#output\_kub\_vsts\_campaign\_orchestrator\_role\_arn) | IAM roles for K8S |
| <a name="output_kub_vsts_ci_service_role_arn"></a> [kub\_vsts\_ci\_service\_role\_arn](#output\_kub\_vsts\_ci\_service\_role\_arn) | n/a |
| <a name="output_kub_vsts_content_service_role_arn"></a> [kub\_vsts\_content\_service\_role\_arn](#output\_kub\_vsts\_content\_service\_role\_arn) | n/a |
| <a name="output_kub_vsts_crypto_service_role_arn"></a> [kub\_vsts\_crypto\_service\_role\_arn](#output\_kub\_vsts\_crypto\_service\_role\_arn) | n/a |
| <a name="output_kub_vsts_device_gateway_role_arn"></a> [kub\_vsts\_device\_gateway\_role\_arn](#output\_kub\_vsts\_device\_gateway\_role\_arn) | n/a |
| <a name="output_kub_vsts_dim_service_role_arn"></a> [kub\_vsts\_dim\_service\_role\_arn](#output\_kub\_vsts\_dim\_service\_role\_arn) | n/a |
| <a name="output_kub_vsts_event_scheduler_role_arn"></a> [kub\_vsts\_event\_scheduler\_role\_arn](#output\_kub\_vsts\_event\_scheduler\_role\_arn) | n/a |
| <a name="output_kub_vsts_gp_service_role_arn"></a> [kub\_vsts\_gp\_service\_role\_arn](#output\_kub\_vsts\_gp\_service\_role\_arn) | n/a |
| <a name="output_kub_vsts_kcss_service_role_arn"></a> [kub\_vsts\_kcss\_service\_role\_arn](#output\_kub\_vsts\_kcss\_service\_role\_arn) | n/a |
| <a name="output_kub_vsts_key_service_role_arn"></a> [kub\_vsts\_key\_service\_role\_arn](#output\_kub\_vsts\_key\_service\_role\_arn) | n/a |
| <a name="output_kub_vsts_notification_service_role_arn"></a> [kub\_vsts\_notification\_service\_role\_arn](#output\_kub\_vsts\_notification\_service\_role\_arn) | n/a |
| <a name="output_kub_vsts_proxy_applet_service_role_arn"></a> [kub\_vsts\_proxy\_applet\_service\_role\_arn](#output\_kub\_vsts\_proxy\_applet\_service\_role\_arn) | n/a |
| <a name="output_kub_vsts_script_executor_role_arn"></a> [kub\_vsts\_script\_executor\_role\_arn](#output\_kub\_vsts\_script\_executor\_role\_arn) | n/a |
| <a name="output_kub_vsts_sms_service_role_arn"></a> [kub\_vsts\_sms\_service\_role\_arn](#output\_kub\_vsts\_sms\_service\_role\_arn) | n/a |
| <a name="output_kub_vsts_statistic_service_role_arn"></a> [kub\_vsts\_statistic\_service\_role\_arn](#output\_kub\_vsts\_statistic\_service\_role\_arn) | n/a |
| <a name="output_kub_vsts_user_service_role_arn"></a> [kub\_vsts\_user\_service\_role\_arn](#output\_kub\_vsts\_user\_service\_role\_arn) | n/a |
| <a name="output_lambda_env_dynamo_grouped_commands_table"></a> [lambda\_env\_dynamo\_grouped\_commands\_table](#output\_lambda\_env\_dynamo\_grouped\_commands\_table) | tables for lambda function |
| <a name="output_lambda_trigger_dynamodb_table"></a> [lambda\_trigger\_dynamodb\_table](#output\_lambda\_trigger\_dynamodb\_table) | n/a |
| <a name="output_mail_sender_address"></a> [mail\_sender\_address](#output\_mail\_sender\_address) | n/a |
| <a name="output_namespace"></a> [namespace](#output\_namespace) | n/a |
| <a name="output_openldap_admin_passwd"></a> [openldap\_admin\_passwd](#output\_openldap\_admin\_passwd) | n/a |
| <a name="output_openldap_ec2_private_ip"></a> [openldap\_ec2\_private\_ip](#output\_openldap\_ec2\_private\_ip) | n/a |
| <a name="output_openldap_login"></a> [openldap\_login](#output\_openldap\_login) | n/a |
| <a name="output_openldap_partition_suffix"></a> [openldap\_partition\_suffix](#output\_openldap\_partition\_suffix) | n/a |
| <a name="output_openldap_url"></a> [openldap\_url](#output\_openldap\_url) | n/a |
| <a name="output_policy_thing_backend_client_name"></a> [policy\_thing\_backend\_client\_name](#output\_policy\_thing\_backend\_client\_name) | n/a |
| <a name="output_prefix"></a> [prefix](#output\_prefix) | n/a |
| <a name="output_projectname"></a> [projectname](#output\_projectname) | n/a |
| <a name="output_s3_device_configuration"></a> [s3\_device\_configuration](#output\_s3\_device\_configuration) | n/a |
| <a name="output_s3_static_documentation"></a> [s3\_static\_documentation](#output\_s3\_static\_documentation) | n/a |
| <a name="output_vpc_cidr_starting_ip"></a> [vpc\_cidr\_starting\_ip](#output\_vpc\_cidr\_starting\_ip) | n/a |