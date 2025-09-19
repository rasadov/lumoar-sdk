# UserApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**changePasswordV1UserPasswordChangePatch**](#changepasswordv1userpasswordchangepatch) | **PATCH** /v1/user/password/change | Change Password|
|[**deleteUserV1UserDeleteDelete**](#deleteuserv1userdeletedelete) | **DELETE** /v1/user/delete | Delete User|
|[**getUserDashV1UserMeDashGet**](#getuserdashv1usermedashget) | **GET** /v1/user/me/dash | Get User Dash|
|[**getUserV1UserMeGet**](#getuserv1usermeget) | **GET** /v1/user/me | Get User|
|[**updateUserV1UserUpdatePatch**](#updateuserv1userupdatepatch) | **PATCH** /v1/user/update | Update User|

# **changePasswordV1UserPasswordChangePatch**
> Details changePasswordV1UserPasswordChangePatch(updatePassword)

Change user password

### Example

```typescript
import {
    UserApi,
    Configuration,
    UpdatePassword
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let updatePassword: UpdatePassword; //
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.changePasswordV1UserPasswordChangePatch(
    updatePassword,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updatePassword** | **UpdatePassword**|  | |
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Details**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteUserV1UserDeleteDelete**
> Details deleteUserV1UserDeleteDelete()

Delete user

### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteUserV1UserDeleteDelete(
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Details**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUserDashV1UserMeDashGet**
> UserWithRelations getUserDashV1UserMeDashGet()

Get current user with relations

### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getUserDashV1UserMeDashGet(
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**UserWithRelations**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUserV1UserMeGet**
> UserInDBBase getUserV1UserMeGet()

Get current user

### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getUserV1UserMeGet(
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**UserInDBBase**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateUserV1UserUpdatePatch**
> Details updateUserV1UserUpdatePatch(userUpdate)

Update user

### Example

```typescript
import {
    UserApi,
    Configuration,
    UserUpdate
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let userUpdate: UserUpdate; //
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateUserV1UserUpdatePatch(
    userUpdate,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userUpdate** | **UserUpdate**|  | |
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Details**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

