# BlockListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Blocks** | [**[]Block**](Block.md) |  | 
**Total** | **int32** |  | 

## Methods

### NewBlockListResponse

`func NewBlockListResponse(blocks []Block, total int32, ) *BlockListResponse`

NewBlockListResponse instantiates a new BlockListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBlockListResponseWithDefaults

`func NewBlockListResponseWithDefaults() *BlockListResponse`

NewBlockListResponseWithDefaults instantiates a new BlockListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBlocks

`func (o *BlockListResponse) GetBlocks() []Block`

GetBlocks returns the Blocks field if non-nil, zero value otherwise.

### GetBlocksOk

`func (o *BlockListResponse) GetBlocksOk() (*[]Block, bool)`

GetBlocksOk returns a tuple with the Blocks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlocks

`func (o *BlockListResponse) SetBlocks(v []Block)`

SetBlocks sets Blocks field to given value.


### GetTotal

`func (o *BlockListResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *BlockListResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *BlockListResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


