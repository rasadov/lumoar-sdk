# LoginSchema

Login schema for user authentication. Attributes:     - email: EmailStr     - password: SecretStr     - turnstile_token: str

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **string** |  | [default to undefined]
**password** | **string** |  | [default to undefined]
**turnstile_token** | **string** |  | [default to undefined]

## Example

```typescript
import { LoginSchema } from './api';

const instance: LoginSchema = {
    email,
    password,
    turnstile_token,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
