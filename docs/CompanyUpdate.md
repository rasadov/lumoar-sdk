# CompanyUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**industry** | **string** |  | [optional] [default to undefined]
**employee_count** | **number** |  | [optional] [default to undefined]
**domain** | **string** |  | [optional] [default to undefined]
**tools_used** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**compliance_goal** | [**ComplianceGoal**](ComplianceGoal.md) |  | [optional] [default to undefined]
**readiness_score** | **number** |  | [optional] [default to undefined]
**audit_due_date** | **string** |  | [optional] [default to undefined]
**is_audit_mode** | **boolean** |  | [optional] [default to undefined]
**timezone** | **string** |  | [optional] [default to undefined]
**logo_url** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { CompanyUpdate } from './api';

const instance: CompanyUpdate = {
    id,
    name,
    industry,
    employee_count,
    domain,
    tools_used,
    compliance_goal,
    readiness_score,
    audit_due_date,
    is_audit_mode,
    timezone,
    logo_url,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
