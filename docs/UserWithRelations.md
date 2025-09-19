# UserWithRelations


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [default to undefined]
**email** | **string** |  | [default to undefined]
**phone** | **string** |  | [optional] [default to undefined]
**role** | **string** |  | [optional] [default to 'customer']
**company_permissions** | [**Array&lt;UserPermissionsWithCompany&gt;**](UserPermissionsWithCompany.md) |  | [default to undefined]

## Example

```typescript
import { UserWithRelations } from './api';

const instance: UserWithRelations = {
    name,
    email,
    phone,
    role,
    company_permissions,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
