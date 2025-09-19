# CompanyWithControls


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [default to undefined]
**industry** | **string** |  | [default to undefined]
**employee_count** | **number** |  | [default to undefined]
**domain** | **string** |  | [default to undefined]
**tools_used** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**plan** | **string** |  | [optional] [default to undefined]
**status** | **string** |  | [optional] [default to undefined]
**compliance_goal** | [**ComplianceGoal**](ComplianceGoal.md) |  | [optional] [default to undefined]
**readiness_score** | **number** |  | [optional] [default to undefined]
**audit_due_date** | **string** |  | [optional] [default to undefined]
**is_audit_mode** | **boolean** |  | [optional] [default to false]
**timezone** | **string** |  | [optional] [default to 'UTC']
**logo_url** | **string** |  | [optional] [default to undefined]
**id** | **string** |  | [default to undefined]
**updated_at** | **string** |  | [default to undefined]
**controls** | [**Array&lt;ControlWithEvidences&gt;**](ControlWithEvidences.md) |  | [default to undefined]

## Example

```typescript
import { CompanyWithControls } from './api';

const instance: CompanyWithControls = {
    name,
    industry,
    employee_count,
    domain,
    tools_used,
    plan,
    status,
    compliance_goal,
    readiness_score,
    audit_due_date,
    is_audit_mode,
    timezone,
    logo_url,
    id,
    updated_at,
    controls,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
