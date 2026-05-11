# UploadChunkedBlockResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**BlockHash** | **string** |  | 
**Uploaded** | **bool** |  | 
**BlocksRemaining** | **int32** |  | 
**Progress** | **float64** | Percent complete, 0–100. | 

## Methods

### NewUploadChunkedBlockResponse

`func NewUploadChunkedBlockResponse(blockHash string, uploaded bool, blocksRemaining int32, progress float64, ) *UploadChunkedBlockResponse`

NewUploadChunkedBlockResponse instantiates a new UploadChunkedBlockResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUploadChunkedBlockResponseWithDefaults

`func NewUploadChunkedBlockResponseWithDefaults() *UploadChunkedBlockResponse`

NewUploadChunkedBlockResponseWithDefaults instantiates a new UploadChunkedBlockResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBlockHash

`func (o *UploadChunkedBlockResponse) GetBlockHash() string`

GetBlockHash returns the BlockHash field if non-nil, zero value otherwise.

### GetBlockHashOk

`func (o *UploadChunkedBlockResponse) GetBlockHashOk() (*string, bool)`

GetBlockHashOk returns a tuple with the BlockHash field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlockHash

`func (o *UploadChunkedBlockResponse) SetBlockHash(v string)`

SetBlockHash sets BlockHash field to given value.


### GetUploaded

`func (o *UploadChunkedBlockResponse) GetUploaded() bool`

GetUploaded returns the Uploaded field if non-nil, zero value otherwise.

### GetUploadedOk

`func (o *UploadChunkedBlockResponse) GetUploadedOk() (*bool, bool)`

GetUploadedOk returns a tuple with the Uploaded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUploaded

`func (o *UploadChunkedBlockResponse) SetUploaded(v bool)`

SetUploaded sets Uploaded field to given value.


### GetBlocksRemaining

`func (o *UploadChunkedBlockResponse) GetBlocksRemaining() int32`

GetBlocksRemaining returns the BlocksRemaining field if non-nil, zero value otherwise.

### GetBlocksRemainingOk

`func (o *UploadChunkedBlockResponse) GetBlocksRemainingOk() (*int32, bool)`

GetBlocksRemainingOk returns a tuple with the BlocksRemaining field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlocksRemaining

`func (o *UploadChunkedBlockResponse) SetBlocksRemaining(v int32)`

SetBlocksRemaining sets BlocksRemaining field to given value.


### GetProgress

`func (o *UploadChunkedBlockResponse) GetProgress() float64`

GetProgress returns the Progress field if non-nil, zero value otherwise.

### GetProgressOk

`func (o *UploadChunkedBlockResponse) GetProgressOk() (*float64, bool)`

GetProgressOk returns a tuple with the Progress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProgress

`func (o *UploadChunkedBlockResponse) SetProgress(v float64)`

SetProgress sets Progress field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


