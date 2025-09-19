# CompanyApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createCompanyV1CompanyCreatePost**](#createcompanyv1companycreatepost) | **POST** /v1/company/create | Create Company|
|[**getCompaniesV1CompanyListGet**](#getcompaniesv1companylistget) | **GET** /v1/company/list | Get Companies|
|[**getCompanyV1CompanyGetCompanyIdGet**](#getcompanyv1companygetcompanyidget) | **GET** /v1/company/get/{company_id} | Get Company|
|[**getControlsV1CompanyControlsCompanyIdGet**](#getcontrolsv1companycontrolscompanyidget) | **GET** /v1/company/controls/{company_id} | Get Controls|
|[**getPoliciesV1CompanyPoliciesGet**](#getpoliciesv1companypoliciesget) | **GET** /v1/company/policies | Get Policies|
|[**updateCompanyV1CompanyUpdatePatch**](#updatecompanyv1companyupdatepatch) | **PATCH** /v1/company/update | Update Company|

# **createCompanyV1CompanyCreatePost**
> CompanyInDBBase createCompanyV1CompanyCreatePost(companyCreate)


### Example

```typescript
import {
    CompanyApi,
    Configuration,
    CompanyCreate
} from './api';

const configuration = new Configuration();
const apiInstance = new CompanyApi(configuration);

let companyCreate: CompanyCreate; //
let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createCompanyV1CompanyCreatePost(
    companyCreate,
    authorization,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **companyCreate** | **CompanyCreate**|  | |
| **authorization** | [**string**] |  | (optional) defaults to undefined|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**CompanyInDBBase**

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

# **getCompaniesV1CompanyListGet**
> Array<CompanyInDBBase> getCompaniesV1CompanyListGet()


### Example

```typescript
import {
    CompanyApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new CompanyApi(configuration);

let page: number; // (optional) (default to 1)
let limit: number; // (optional) (default to 10)
let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getCompaniesV1CompanyListGet(
    page,
    limit,
    authorization,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **page** | [**number**] |  | (optional) defaults to 1|
| **limit** | [**number**] |  | (optional) defaults to 10|
| **authorization** | [**string**] |  | (optional) defaults to undefined|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Array<CompanyInDBBase>**

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

# **getCompanyV1CompanyGetCompanyIdGet**
> CompanyWithRoles getCompanyV1CompanyGetCompanyIdGet()


### Example

```typescript
import {
    CompanyApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new CompanyApi(configuration);

let companyId: string; // (default to undefined)
let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getCompanyV1CompanyGetCompanyIdGet(
    companyId,
    authorization,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **companyId** | [**string**] |  | defaults to undefined|
| **authorization** | [**string**] |  | (optional) defaults to undefined|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**CompanyWithRoles**

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

# **getControlsV1CompanyControlsCompanyIdGet**
> CompanyWithControls getControlsV1CompanyControlsCompanyIdGet()


### Example

```typescript
import {
    CompanyApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new CompanyApi(configuration);

let companyId: string; // (default to undefined)
let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getControlsV1CompanyControlsCompanyIdGet(
    companyId,
    authorization,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **companyId** | [**string**] |  | defaults to undefined|
| **authorization** | [**string**] |  | (optional) defaults to undefined|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**CompanyWithControls**

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

# **getPoliciesV1CompanyPoliciesGet**
> Array<PolicyRead> getPoliciesV1CompanyPoliciesGet()


### Example

```typescript
import {
    CompanyApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new CompanyApi(configuration);

let page: number; // (optional) (default to 1)
let limit: number; // (optional) (default to 10)
let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getPoliciesV1CompanyPoliciesGet(
    page,
    limit,
    authorization,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **page** | [**number**] |  | (optional) defaults to 1|
| **limit** | [**number**] |  | (optional) defaults to 10|
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

# **updateCompanyV1CompanyUpdatePatch**
> CompanyInDBBase updateCompanyV1CompanyUpdatePatch(companyUpdate)


### Example

```typescript
import {
    CompanyApi,
    Configuration,
    CompanyUpdate
} from './api';

const configuration = new Configuration();
const apiInstance = new CompanyApi(configuration);

let companyUpdate: CompanyUpdate; //
let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateCompanyV1CompanyUpdatePatch(
    companyUpdate,
    authorization,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **companyUpdate** | **CompanyUpdate**|  | |
| **authorization** | [**string**] |  | (optional) defaults to undefined|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**CompanyInDBBase**

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

