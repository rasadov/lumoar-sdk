# PaymentsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getCheckoutSessionPaymentsCheckoutGet**](#getcheckoutsessionpaymentscheckoutget) | **GET** /payments/checkout | Get Checkout Session|
|[**getCustomerManagementSessionPaymentsCustomerManagementGet**](#getcustomermanagementsessionpaymentscustomermanagementget) | **GET** /payments/customer/management | Get Customer Management Session|
|[**webhookPaymentsWebhookPost**](#webhookpaymentswebhookpost) | **POST** /payments/webhook | Webhook|

# **getCheckoutSessionPaymentsCheckoutGet**
> ResponseGetCheckoutSessionPaymentsCheckoutGet getCheckoutSessionPaymentsCheckoutGet()


### Example

```typescript
import {
    PaymentsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PaymentsApi(configuration);

let userId: string; // (default to undefined)
let companyId: string; // (default to undefined)
let productId: string; // (default to undefined)

const { status, data } = await apiInstance.getCheckoutSessionPaymentsCheckoutGet(
    userId,
    companyId,
    productId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**string**] |  | defaults to undefined|
| **companyId** | [**string**] |  | defaults to undefined|
| **productId** | [**string**] |  | defaults to undefined|


### Return type

**ResponseGetCheckoutSessionPaymentsCheckoutGet**

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

# **getCustomerManagementSessionPaymentsCustomerManagementGet**
> ResponseGetCustomerManagementSessionPaymentsCustomerManagementGet getCustomerManagementSessionPaymentsCustomerManagementGet()


### Example

```typescript
import {
    PaymentsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PaymentsApi(configuration);

let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getCustomerManagementSessionPaymentsCustomerManagementGet(
    authorization,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **authorization** | [**string**] |  | (optional) defaults to undefined|
| **sessionId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**ResponseGetCustomerManagementSessionPaymentsCustomerManagementGet**

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

# **webhookPaymentsWebhookPost**
> any webhookPaymentsWebhookPost()


### Example

```typescript
import {
    PaymentsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new PaymentsApi(configuration);

const { status, data } = await apiInstance.webhookPaymentsWebhookPost();
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

