# PolicyCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Name of the policy | [default to undefined]
**type** | **string** | Type of policy (e.g., \&#39;security\&#39;, \&#39;privacy\&#39;) | [default to undefined]
**content** | **{ [key: string]: any; }** | Policy content as a JSON object | [default to undefined]
**company_id** | **string** | UUID of the company this policy belongs to | [default to undefined]

## Example

```typescript
import { PolicyCreate } from './api';

const instance: PolicyCreate = {
    name,
    type,
    content,
    company_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
