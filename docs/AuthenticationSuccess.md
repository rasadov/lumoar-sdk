# AuthenticationSuccess

Authentication success response schema. Attributes:     - access_token: str     - token_type: str     - user_id: str     - role: str

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**detail** | **{ [key: string]: string; }** |  | [default to undefined]
**access_token** | **string** |  | [default to undefined]
**user** | [**UserInDBBase**](UserInDBBase.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AuthenticationSuccess } from './api';

const instance: AuthenticationSuccess = {
    detail,
    access_token,
    user,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
