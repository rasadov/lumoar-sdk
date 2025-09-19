# RegisterSchema

Register schema for user registration. Attributes:     - email: EmailStr     - password: SecretStr     - password_repeat: SecretStr     - name: str | None     - phone: str | None     - turnstile_token: str

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **string** |  | [default to undefined]
**password** | **string** |  | [default to undefined]
**turnstile_token** | **string** |  | [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**phone** | **string** |  | [optional] [default to undefined]
**password_repeat** | **string** |  | [default to undefined]

## Example

```typescript
import { RegisterSchema } from './api';

const instance: RegisterSchema = {
    email,
    password,
    turnstile_token,
    name,
    phone,
    password_repeat,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
