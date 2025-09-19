# EvidenceApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**deleteEvidenceV1EvidenceDeleteDelete**](#deleteevidencev1evidencedeletedelete) | **DELETE** /v1/evidence/delete | Delete Evidence|
|[**getEvidenceFilesV1EvidenceFileEvidenceIdGet**](#getevidencefilesv1evidencefileevidenceidget) | **GET** /v1/evidence/file/{evidence_id} | Get Evidence Files|
|[**listCompanyEvidenceV1EvidenceCompanyCompanyIdGet**](#listcompanyevidencev1evidencecompanycompanyidget) | **GET** /v1/evidence/company/{company_id} | List Company Evidence|
|[**updateEvidenceV1EvidenceUpdatePut**](#updateevidencev1evidenceupdateput) | **PUT** /v1/evidence/update | Update Evidence|
|[**uploadEvidenceV1EvidenceUploadPost**](#uploadevidencev1evidenceuploadpost) | **POST** /v1/evidence/upload | Upload Evidence|

# **deleteEvidenceV1EvidenceDeleteDelete**
> deleteEvidenceV1EvidenceDeleteDelete()


### Example

```typescript
import {
    EvidenceApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new EvidenceApi(configuration);

let evidenceId: string; // (default to undefined)
let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteEvidenceV1EvidenceDeleteDelete(
    evidenceId,
    authorization,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **evidenceId** | [**string**] |  | defaults to undefined|
| **authorization** | [**string**] |  | (optional) defaults to undefined|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getEvidenceFilesV1EvidenceFileEvidenceIdGet**
> Array<FileDownload> getEvidenceFilesV1EvidenceFileEvidenceIdGet()


### Example

```typescript
import {
    EvidenceApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new EvidenceApi(configuration);

let evidenceId: string; // (default to undefined)
let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getEvidenceFilesV1EvidenceFileEvidenceIdGet(
    evidenceId,
    authorization,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **evidenceId** | [**string**] |  | defaults to undefined|
| **authorization** | [**string**] |  | (optional) defaults to undefined|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Array<FileDownload>**

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

# **listCompanyEvidenceV1EvidenceCompanyCompanyIdGet**
> Array<EvidenceBase> listCompanyEvidenceV1EvidenceCompanyCompanyIdGet()


### Example

```typescript
import {
    EvidenceApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new EvidenceApi(configuration);

let companyId: string; // (default to undefined)
let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.listCompanyEvidenceV1EvidenceCompanyCompanyIdGet(
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

**Array<EvidenceBase>**

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

# **updateEvidenceV1EvidenceUpdatePut**
> EvidenceBase updateEvidenceV1EvidenceUpdatePut()


### Example

```typescript
import {
    EvidenceApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new EvidenceApi(configuration);

let evidenceId: string; // (default to undefined)
let text: string; // (default to undefined)
let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateEvidenceV1EvidenceUpdatePut(
    evidenceId,
    text,
    authorization,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **evidenceId** | [**string**] |  | defaults to undefined|
| **text** | [**string**] |  | defaults to undefined|
| **authorization** | [**string**] |  | (optional) defaults to undefined|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**EvidenceBase**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **uploadEvidenceV1EvidenceUploadPost**
> EvidenceBase uploadEvidenceV1EvidenceUploadPost()


### Example

```typescript
import {
    EvidenceApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new EvidenceApi(configuration);

let companyId: string; // (default to undefined)
let controlId: string; // (default to undefined)
let file: File; // (default to undefined)
let text: string; // (default to undefined)
let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.uploadEvidenceV1EvidenceUploadPost(
    companyId,
    controlId,
    file,
    text,
    authorization,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **companyId** | [**string**] |  | defaults to undefined|
| **controlId** | [**string**] |  | defaults to undefined|
| **file** | [**File**] |  | defaults to undefined|
| **text** | [**string**] |  | defaults to undefined|
| **authorization** | [**string**] |  | (optional) defaults to undefined|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**EvidenceBase**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

