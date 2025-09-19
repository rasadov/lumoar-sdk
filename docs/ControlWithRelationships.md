# ControlWithRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**framework_control** | [**FrameworkControlsBase**](FrameworkControlsBase.md) |  | [default to undefined]
**status** | **string** |  | [optional] [default to undefined]
**note** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]
**company** | [**CompanyInDBBase**](CompanyInDBBase.md) |  | [default to undefined]
**evidences** | [**Array&lt;EvidenceBase&gt;**](EvidenceBase.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ControlWithRelationships } from './api';

const instance: ControlWithRelationships = {
    id,
    framework_control,
    status,
    note,
    updated_at,
    company,
    evidences,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
