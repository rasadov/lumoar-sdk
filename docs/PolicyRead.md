# PolicyRead


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique identifier for the policy | [default to undefined]
**name** | **string** | Name of the policy | [default to undefined]
**type** | **string** | Type of policy | [default to undefined]
**content** | **{ [key: string]: any; }** | Policy content | [default to undefined]
**company_id** | **string** | UUID of the associated company | [default to undefined]
**created_by** | **string** | UUID of the user who created the policy | [default to undefined]
**created_at** | **string** | Timestamp when the policy was created | [default to undefined]

## Example

```typescript
import { PolicyRead } from './api';

const instance: PolicyRead = {
    id,
    name,
    type,
    content,
    company_id,
    created_by,
    created_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
