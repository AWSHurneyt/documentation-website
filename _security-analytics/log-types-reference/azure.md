---
layout: default
title: Azure
parent: Supported log types
nav_order: 29
---

# Azure

The `azure` log type monitors log data for cloud applications managed by Azure Cloud Services.

The following code snippet contains all `raw_field` and `ecs` mappings for this log type:

```json
"mappings": [
    {
      "raw_field":"Resultdescription",
      "ecs":"azure.signinlogs.result_description"
    },
    {
      "raw_field":"eventSource",
      "ecs":"eventSource"
    },
    {
      "raw_field":"eventName",
      "ecs":"eventName"
    },
    {
      "raw_field":"Status",
      "ecs":"azure.platformlogs.status"
    },
    {
      "raw_field":"LoggedByService",
      "ecs":"azure.auditlogs.properties.logged_by_service"
    },
    {
      "raw_field":"properties_message",
      "ecs":"properties_message"
    },
    {
      "raw_field":"status",
      "ecs":"azure.platformlogs.status"
    },
    {
      "raw_field":"TargetUserName",
      "ecs":"azure.signinlogs.properties.user_id"
    },
    {
      "raw_field":"creationTime",
      "ecs":"timestamp"
    },
    {
      "raw_field":"Category",
      "ecs":"azure.activitylogs.category"
    },
    {
      "raw_field":"OperationName",
      "ecs":"azure.platformlogs.operation_name"
    },
    {
      "raw_field":"ModifiedProperties_NewValue",
      "ecs":"modified_properties.new_value"
    },
    {
      "raw_field":"ResourceProviderValue",
      "ecs":"azure.resource.provider"
    },
    {
      "raw_field":"conditionalAccessStatus",
      "ecs":"azure.signinlogs.properties.conditional_access_status"
    },
    {
      "raw_field":"SearchFilter",
      "ecs":"search_filter"
    },
    {
      "raw_field":"Operation",
      "ecs":"azure.platformlogs.operation_name"
    },
    {
      "raw_field":"ResultType",
      "ecs":"azure.platformlogs.result_type"
    },
    {
      "raw_field":"DeviceDetail_isCompliant",
      "ecs":"azure.signinlogs.properties.device_detail.is_compliant"
    },
    {
      "raw_field":"ResourceDisplayName",
      "ecs":"resource_display_name"
    },
    {
      "raw_field":"AuthenticationRequirement",
      "ecs":"azure.signinlogs.properties.authentication_requirement"
    },
    {
      "raw_field":"TargetResources",
      "ecs":"target_resources"
    },
    {
      "raw_field":"Workload",
      "ecs":"Workload"
    },
    {
      "raw_field":"DeviceDetail_deviceId",
      "ecs":"azure.signinlogs.properties.device_detail.device_id"
    },
    {
      "raw_field":"OperationNameValue",
      "ecs":"azure.platformlogs.operation_name"
    },
    {
      "raw_field":"ResourceId",
      "ecs":"azure.signinlogs.properties.resource_id"
    },
    {
      "raw_field":"ResultDescription",
      "ecs":"azure.signinlogs.result_description"
    },
    {
      "raw_field":"EventID",
      "ecs":"EventID"
    },
    {
      "raw_field":"NetworkLocationDetails",
      "ecs":"azure.signinlogs.properties.network_location_details"
    },
    {
      "raw_field":"CategoryValue",
      "ecs":"azure.activitylogs.category"
    },
    {
      "raw_field":"ActivityDisplayName",
      "ecs":"azure.auditlogs.properties.activity_display_name"
    },
    {
      "raw_field":"Initiatedby",
      "ecs":"azure.activitylogs.identity.claims_initiated_by_user.name"
    },
    {
      "raw_field":"Count",
      "ecs":"Count"
    },
    {
      "raw_field":"ResourceTenantId",
      "ecs":"azure.signinlogs.properties.resource_tenant_id"
    },
    {
      "raw_field":"failure_status_reason",
      "ecs":"failure_status_reason"
    },
    {
      "raw_field":"AppId",
      "ecs":"azure.signinlogs.properties.app_id"
    },
    {
      "raw_field":"properties.message",
      "ecs":"properties.message"
    },
    {
      "raw_field":"ClientApp",
      "ecs":"azure.signinlogs.properties.client_app_used"
    },
    {
      "raw_field":"ActivityDetails",
      "ecs":"ActivityDetails"
    },
    {
      "raw_field":"Target",
      "ecs":"Target"
    },
    {
      "raw_field":"DeviceDetail.trusttype",
      "ecs":"azure.signinlogs.properties.device_detail.trust_type"
    },
    {
      "raw_field":"HomeTenantId",
      "ecs":"azure.signinlogs.properties.home_tenant_id"
    },
    {
      "raw_field":"ConsentContext.IsAdminConsent",
      "ecs":"ConsentContext.IsAdminConsent"
    },
    {
      "raw_field":"InitiatedBy",
      "ecs":"InitiatedBy"
    },
    {
      "raw_field":"ActivityType",
      "ecs":"azure.auditlogs.properties.activity_display_name"
    },
    {
      "raw_field":"operationName",
      "ecs":"azure.activitylogs.operation_name"
    },
    {
      "raw_field":"ModifiedProperties{}.NewValue",
      "ecs":"modified_properties.new_value"
    },
    {
      "raw_field":"userAgent",
      "ecs":"user_agent.name"
    },
    {
      "raw_field":"RiskState",
      "ecs":"azure.signinlogs.properties.risk_state"
    },
    {
      "raw_field":"Username",
      "ecs":"azure.activitylogs.identity.claims_initiated_by_user.name"
    },
    {
      "raw_field":"DeviceDetail.deviceId",
      "ecs":"azure.signinlogs.properties.device_detail.device_id"
    },
    {
      "raw_field":"DeviceDetail.isCompliant",
      "ecs":"azure.signinlogs.properties.device_detail.is_compliant"
    },
    {
      "raw_field":"Location",
      "ecs":"azure.signinlogs.properties.network_location_details"
    }
  ]
```