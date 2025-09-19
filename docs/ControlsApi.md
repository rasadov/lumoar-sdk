# ControlsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getControlV1ControlsControlIdGet**](#getcontrolv1controlscontrolidget) | **GET** /v1/controls/{control_id} | Get Control|
|[**updateControlV1ControlsUpdatePatch**](#updatecontrolv1controlsupdatepatch) | **PATCH** /v1/controls/update | Update Control|

# **getControlV1ControlsControlIdGet**
> GetControl getControlV1ControlsControlIdGet()


### Example

```typescript
import {
    ControlsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ControlsApi(configuration);

let controlId: string; // (default to undefined)
let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getControlV1ControlsControlIdGet(
    controlId,
    authorization,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **controlId** | [**string**] |  | defaults to undefined|
| **authorization** | [**string**] |  | (optional) defaults to undefined|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**GetControl**

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

# **updateControlV1ControlsUpdatePatch**
> GetControl updateControlV1ControlsUpdatePatch(updateControlSchema)


### Example

```typescript
import {
    ControlsApi,
    Configuration,
    UpdateControlSchema
} from './api';

const configuration = new Configuration();
const apiInstance = new ControlsApi(configuration);

let updateControlSchema: UpdateControlSchema; //
let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateControlV1ControlsUpdatePatch(
    updateControlSchema,
    authorization,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateControlSchema** | **UpdateControlSchema**|  | |
| **authorization** | [**string**] |  | (optional) defaults to undefined|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**GetControl**

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

