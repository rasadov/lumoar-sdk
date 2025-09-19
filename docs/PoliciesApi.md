# PoliciesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createPolicyV1PoliciesCreatePost**](#createpolicyv1policiescreatepost) | **POST** /v1/policies/create | Create Policy|
|[**deletePolicyV1PoliciesPolicyIdDelete**](#deletepolicyv1policiespolicyiddelete) | **DELETE** /v1/policies/{policy_id} | Delete Policy|
|[**getCompanyPoliciesV1PoliciesCompanyCompanyIdGet**](#getcompanypoliciesv1policiescompanycompanyidget) | **GET** /v1/policies/company/{company_id} | Get Company Policies|
|[**getPolicyV1PoliciesPolicyIdGet**](#getpolicyv1policiespolicyidget) | **GET** /v1/policies/{policy_id} | Get Policy|
|[**updatePolicyV1PoliciesPolicyIdPut**](#updatepolicyv1policiespolicyidput) | **PUT** /v1/policies/{policy_id} | Update Policy|

# **createPolicyV1PoliciesCreatePost**
> PolicyRead createPolicyV1PoliciesCreatePost(policyCreate)


### Example

```typescript
import {
    PoliciesApi,
    Configuration,
    PolicyCreate
} from './api';

const configuration = new Configuration();
const apiInstance = new PoliciesApi(configuration);

let policyCreate: PolicyCreate; //
let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createPolicyV1PoliciesCreatePost(
    policyCreate,
    authorization,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **policyCreate** | **PolicyCreate**|  | |
| **authorization** | [**string**] |  | (optional) defaults to undefined|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**PolicyRead**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deletePolicyV1PoliciesPolicyIdDelete**
> deletePolicyV1PoliciesPolicyIdDelete()


### Example

```typescript
import {
    PoliciesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PoliciesApi(configuration);

let policyId: string; // (default to undefined)
let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deletePolicyV1PoliciesPolicyIdDelete(
    policyId,
    authorization,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **policyId** | [**string**] |  | defaults to undefined|
| **authorization** | [**string**] |  | (optional) defaults to undefined|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getCompanyPoliciesV1PoliciesCompanyCompanyIdGet**
> Array<PolicyRead> getCompanyPoliciesV1PoliciesCompanyCompanyIdGet()


### Example

```typescript
import {
    PoliciesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PoliciesApi(configuration);

let companyId: string; // (default to undefined)
let skip: number; //Number of records to skip for pagination (optional) (default to 0)
let limit: number; //Maximum number of records to return (optional) (default to 100)
let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getCompanyPoliciesV1PoliciesCompanyCompanyIdGet(
    companyId,
    skip,
    limit,
    authorization,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **companyId** | [**string**] |  | defaults to undefined|
| **skip** | [**number**] | Number of records to skip for pagination | (optional) defaults to 0|
| **limit** | [**number**] | Maximum number of records to return | (optional) defaults to 100|
| **authorization** | [**string**] |  | (optional) defaults to undefined|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Array<PolicyRead>**

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

# **getPolicyV1PoliciesPolicyIdGet**
> PolicyRead getPolicyV1PoliciesPolicyIdGet()


### Example

```typescript
import {
    PoliciesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PoliciesApi(configuration);

let policyId: string; // (default to undefined)

const { status, data } = await apiInstance.getPolicyV1PoliciesPolicyIdGet(
    policyId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **policyId** | [**string**] |  | defaults to undefined|


### Return type

**PolicyRead**

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

# **updatePolicyV1PoliciesPolicyIdPut**
> PolicyRead updatePolicyV1PoliciesPolicyIdPut(policyUpdate)


### Example

```typescript
import {
    PoliciesApi,
    Configuration,
    PolicyUpdate
} from './api';

const configuration = new Configuration();
const apiInstance = new PoliciesApi(configuration);

let policyId: string; // (default to undefined)
let policyUpdate: PolicyUpdate; //
let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updatePolicyV1PoliciesPolicyIdPut(
    policyId,
    policyUpdate,
    authorization,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **policyUpdate** | **PolicyUpdate**|  | |
| **policyId** | [**string**] |  | defaults to undefined|
| **authorization** | [**string**] |  | (optional) defaults to undefined|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**PolicyRead**

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

