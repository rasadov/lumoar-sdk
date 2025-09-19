# AuthApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**deleteSessionV1AuthSessionDelete**](#deletesessionv1authsessiondelete) | **DELETE** /v1/auth/session | Delete Session|
|[**deleteSessionsV1AuthSessionsDelete**](#deletesessionsv1authsessionsdelete) | **DELETE** /v1/auth/sessions | Delete Sessions|
|[**getSessionsV1AuthSessionsGet**](#getsessionsv1authsessionsget) | **GET** /v1/auth/sessions | Get Sessions|
|[**githubCallbackV1AuthGithubCallbackPost**](#githubcallbackv1authgithubcallbackpost) | **POST** /v1/auth/github/callback | Github Callback|
|[**githubLoginV1AuthGithubLoginGet**](#githubloginv1authgithubloginget) | **GET** /v1/auth/github/login | Github Login|
|[**googleCallbackV1AuthGoogleCallbackPost**](#googlecallbackv1authgooglecallbackpost) | **POST** /v1/auth/google/callback | Google Callback|
|[**googleLoginV1AuthGoogleLoginGet**](#googleloginv1authgoogleloginget) | **GET** /v1/auth/google/login | Google Login|
|[**loginV1AuthLoginPost**](#loginv1authloginpost) | **POST** /v1/auth/login | Login|
|[**logoutV1AuthLogoutPost**](#logoutv1authlogoutpost) | **POST** /v1/auth/logout | Logout|
|[**registerV1AuthRegisterPost**](#registerv1authregisterpost) | **POST** /v1/auth/register | Register|

# **deleteSessionV1AuthSessionDelete**
> Details deleteSessionV1AuthSessionDelete()

Delete user session

### Example

```typescript
import {
    AuthApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

let sessionIdToDelete: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteSessionV1AuthSessionDelete(
    sessionIdToDelete,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sessionIdToDelete** | [**string**] |  | (optional) defaults to undefined|
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

# **deleteSessionsV1AuthSessionsDelete**
> Details deleteSessionsV1AuthSessionsDelete()

Delete user sessions

### Example

```typescript
import {
    AuthApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteSessionsV1AuthSessionsDelete(
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

# **getSessionsV1AuthSessionsGet**
> Array<{ [key: string]: string | null; }> getSessionsV1AuthSessionsGet()

Get user sessions

### Example

```typescript
import {
    AuthApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getSessionsV1AuthSessionsGet(
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Array<{ [key: string]: string | null; }>**

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

# **githubCallbackV1AuthGithubCallbackPost**
> any githubCallbackV1AuthGithubCallbackPost()

Handles the callback from GitHub OAuth.

### Example

```typescript
import {
    AuthApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

let code: string; // (default to undefined)
let userAgent: string; // (optional) (default to undefined)
let cFConnectingIP: string; // (optional) (default to undefined)
let cFIPCountry: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.githubCallbackV1AuthGithubCallbackPost(
    code,
    userAgent,
    cFConnectingIP,
    cFIPCountry
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **code** | [**string**] |  | defaults to undefined|
| **userAgent** | [**string**] |  | (optional) defaults to undefined|
| **cFConnectingIP** | [**string**] |  | (optional) defaults to undefined|
| **cFIPCountry** | [**string**] |  | (optional) defaults to undefined|


### Return type

**any**

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

# **githubLoginV1AuthGithubLoginGet**
> any githubLoginV1AuthGithubLoginGet()

Redirects to GitHub\'s OAuth consent screen.

### Example

```typescript
import {
    AuthApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

const { status, data } = await apiInstance.githubLoginV1AuthGithubLoginGet();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **googleCallbackV1AuthGoogleCallbackPost**
> any googleCallbackV1AuthGoogleCallbackPost()

Handles the callback from Google OAuth.

### Example

```typescript
import {
    AuthApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

let code: string; // (default to undefined)
let userAgent: string; // (optional) (default to undefined)
let cFConnectingIP: string; // (optional) (default to undefined)
let cFIPCountry: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.googleCallbackV1AuthGoogleCallbackPost(
    code,
    userAgent,
    cFConnectingIP,
    cFIPCountry
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **code** | [**string**] |  | defaults to undefined|
| **userAgent** | [**string**] |  | (optional) defaults to undefined|
| **cFConnectingIP** | [**string**] |  | (optional) defaults to undefined|
| **cFIPCountry** | [**string**] |  | (optional) defaults to undefined|


### Return type

**any**

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

# **googleLoginV1AuthGoogleLoginGet**
> any googleLoginV1AuthGoogleLoginGet()

Redirects to Google\'s OAuth consent screen.

### Example

```typescript
import {
    AuthApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

const { status, data } = await apiInstance.googleLoginV1AuthGoogleLoginGet();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **loginV1AuthLoginPost**
> AuthenticationSuccess loginV1AuthLoginPost(loginSchema)


### Example

```typescript
import {
    AuthApi,
    Configuration,
    LoginSchema
} from './api';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

let loginSchema: LoginSchema; //
let userAgent: string; // (optional) (default to undefined)
let cFConnectingIP: string; // (optional) (default to undefined)
let cFIPCountry: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.loginV1AuthLoginPost(
    loginSchema,
    userAgent,
    cFConnectingIP,
    cFIPCountry
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **loginSchema** | **LoginSchema**|  | |
| **userAgent** | [**string**] |  | (optional) defaults to undefined|
| **cFConnectingIP** | [**string**] |  | (optional) defaults to undefined|
| **cFIPCountry** | [**string**] |  | (optional) defaults to undefined|


### Return type

**AuthenticationSuccess**

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

# **logoutV1AuthLogoutPost**
> Details logoutV1AuthLogoutPost()

Logout user

### Example

```typescript
import {
    AuthApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.logoutV1AuthLogoutPost(
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

# **registerV1AuthRegisterPost**
> AuthenticationSuccess registerV1AuthRegisterPost(registerSchema)


### Example

```typescript
import {
    AuthApi,
    Configuration,
    RegisterSchema
} from './api';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

let registerSchema: RegisterSchema; //
let userAgent: string; // (optional) (default to undefined)
let cFConnectingIP: string; // (optional) (default to undefined)
let cFIPCountry: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.registerV1AuthRegisterPost(
    registerSchema,
    userAgent,
    cFConnectingIP,
    cFIPCountry
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **registerSchema** | **RegisterSchema**|  | |
| **userAgent** | [**string**] |  | (optional) defaults to undefined|
| **cFConnectingIP** | [**string**] |  | (optional) defaults to undefined|
| **cFIPCountry** | [**string**] |  | (optional) defaults to undefined|


### Return type

**AuthenticationSuccess**

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

