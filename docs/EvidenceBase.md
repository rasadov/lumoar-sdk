# EvidenceBase


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**control_id** | **string** |  | [default to undefined]
**expires_at** | **string** |  | [optional] [default to undefined]
**status** | **string** |  | [default to undefined]
**version** | **number** |  | [default to undefined]
**type** | **string** |  | [default to undefined]
**text** | [**EvidenceTextSchema**](EvidenceTextSchema.md) |  | [optional] [default to undefined]
**files** | [**Array&lt;EvidenceFileSchema&gt;**](EvidenceFileSchema.md) |  | [optional] [default to undefined]
**tags** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**uploaded_by** | [**UserBase**](UserBase.md) |  | [optional] [default to undefined]
**submitted_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { EvidenceBase } from './api';

const instance: EvidenceBase = {
    id,
    control_id,
    expires_at,
    status,
    version,
    type,
    text,
    files,
    tags,
    uploaded_by,
    submitted_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
