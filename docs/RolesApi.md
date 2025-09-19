# RolesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**inviteV1RolesInvitesPost**](#invitev1rolesinvitespost) | **POST** /v1/roles/invites | Invite|
|[**removePeopleV1RolesInvitesDelete**](#removepeoplev1rolesinvitesdelete) | **DELETE** /v1/roles/invites | Remove People|

# **inviteV1RolesInvitesPost**
> Details inviteV1RolesInvitesPost(inviteToCompany)

Add people to company

### Example

```typescript
import {
    RolesApi,
    Configuration,
    InviteToCompany
} from './api';

const configuration = new Configuration();
const apiInstance = new RolesApi(configuration);

let inviteToCompany: InviteToCompany; //
let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.inviteV1RolesInvitesPost(
    inviteToCompany,
    authorization,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **inviteToCompany** | **InviteToCompany**|  | |
| **authorization** | [**string**] |  | (optional) defaults to undefined|
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

# **removePeopleV1RolesInvitesDelete**
> Details removePeopleV1RolesInvitesDelete(removeFromCompany)

Remove people from company

### Example

```typescript
import {
    RolesApi,
    Configuration,
    RemoveFromCompany
} from './api';

const configuration = new Configuration();
const apiInstance = new RolesApi(configuration);

let removeFromCompany: RemoveFromCompany; //
let authorization: string; // (optional) (default to undefined)
let sessionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.removePeopleV1RolesInvitesDelete(
    removeFromCompany,
    authorization,
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **removeFromCompany** | **RemoveFromCompany**|  | |
| **authorization** | [**string**] |  | (optional) defaults to undefined|
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

