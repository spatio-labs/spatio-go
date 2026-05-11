# InitChunkedUploadResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**SessionId** | **string** |  | 
**BlocksToUpload** | **[]string** |  | 
**BlocksAlreadyExist** | **[]string** | Blocks the platform already has and the client can skip (content-addressed deduplication).  | 
**DeduplicationPct** | **float64** |  | 
**EstimatedUploadSize** | **int64** |  | 

## Methods

### NewInitChunkedUploadResponse

`func NewInitChunkedUploadResponse(sessionId string, blocksToUpload []string, blocksAlreadyExist []string, deduplicationPct float64, estimatedUploadSize int64, ) *InitChunkedUploadResponse`

NewInitChunkedUploadResponse instantiates a new InitChunkedUploadResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInitChunkedUploadResponseWithDefaults

`func NewInitChunkedUploadResponseWithDefaults() *InitChunkedUploadResponse`

NewInitChunkedUploadResponseWithDefaults instantiates a new InitChunkedUploadResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSessionId

`func (o *InitChunkedUploadResponse) GetSessionId() string`

GetSessionId returns the SessionId field if non-nil, zero value otherwise.

### GetSessionIdOk

`func (o *InitChunkedUploadResponse) GetSessionIdOk() (*string, bool)`

GetSessionIdOk returns a tuple with the SessionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSessionId

`func (o *InitChunkedUploadResponse) SetSessionId(v string)`

SetSessionId sets SessionId field to given value.


### GetBlocksToUpload

`func (o *InitChunkedUploadResponse) GetBlocksToUpload() []string`

GetBlocksToUpload returns the BlocksToUpload field if non-nil, zero value otherwise.

### GetBlocksToUploadOk

`func (o *InitChunkedUploadResponse) GetBlocksToUploadOk() (*[]string, bool)`

GetBlocksToUploadOk returns a tuple with the BlocksToUpload field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlocksToUpload

`func (o *InitChunkedUploadResponse) SetBlocksToUpload(v []string)`

SetBlocksToUpload sets BlocksToUpload field to given value.


### GetBlocksAlreadyExist

`func (o *InitChunkedUploadResponse) GetBlocksAlreadyExist() []string`

GetBlocksAlreadyExist returns the BlocksAlreadyExist field if non-nil, zero value otherwise.

### GetBlocksAlreadyExistOk

`func (o *InitChunkedUploadResponse) GetBlocksAlreadyExistOk() (*[]string, bool)`

GetBlocksAlreadyExistOk returns a tuple with the BlocksAlreadyExist field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlocksAlreadyExist

`func (o *InitChunkedUploadResponse) SetBlocksAlreadyExist(v []string)`

SetBlocksAlreadyExist sets BlocksAlreadyExist field to given value.


### GetDeduplicationPct

`func (o *InitChunkedUploadResponse) GetDeduplicationPct() float64`

GetDeduplicationPct returns the DeduplicationPct field if non-nil, zero value otherwise.

### GetDeduplicationPctOk

`func (o *InitChunkedUploadResponse) GetDeduplicationPctOk() (*float64, bool)`

GetDeduplicationPctOk returns a tuple with the DeduplicationPct field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeduplicationPct

`func (o *InitChunkedUploadResponse) SetDeduplicationPct(v float64)`

SetDeduplicationPct sets DeduplicationPct field to given value.


### GetEstimatedUploadSize

`func (o *InitChunkedUploadResponse) GetEstimatedUploadSize() int64`

GetEstimatedUploadSize returns the EstimatedUploadSize field if non-nil, zero value otherwise.

### GetEstimatedUploadSizeOk

`func (o *InitChunkedUploadResponse) GetEstimatedUploadSizeOk() (*int64, bool)`

GetEstimatedUploadSizeOk returns a tuple with the EstimatedUploadSize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEstimatedUploadSize

`func (o *InitChunkedUploadResponse) SetEstimatedUploadSize(v int64)`

SetEstimatedUploadSize sets EstimatedUploadSize field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


