# BulkMarkReadResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Updated** | **int32** | Number of messages successfully marked. | 
**Failed** | [**[]BulkMarkReadResponseFailedInner**](BulkMarkReadResponseFailedInner.md) |  | 

## Methods

### NewBulkMarkReadResponse

`func NewBulkMarkReadResponse(updated int32, failed []BulkMarkReadResponseFailedInner, ) *BulkMarkReadResponse`

NewBulkMarkReadResponse instantiates a new BulkMarkReadResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBulkMarkReadResponseWithDefaults

`func NewBulkMarkReadResponseWithDefaults() *BulkMarkReadResponse`

NewBulkMarkReadResponseWithDefaults instantiates a new BulkMarkReadResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUpdated

`func (o *BulkMarkReadResponse) GetUpdated() int32`

GetUpdated returns the Updated field if non-nil, zero value otherwise.

### GetUpdatedOk

`func (o *BulkMarkReadResponse) GetUpdatedOk() (*int32, bool)`

GetUpdatedOk returns a tuple with the Updated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdated

`func (o *BulkMarkReadResponse) SetUpdated(v int32)`

SetUpdated sets Updated field to given value.


### GetFailed

`func (o *BulkMarkReadResponse) GetFailed() []BulkMarkReadResponseFailedInner`

GetFailed returns the Failed field if non-nil, zero value otherwise.

### GetFailedOk

`func (o *BulkMarkReadResponse) GetFailedOk() (*[]BulkMarkReadResponseFailedInner, bool)`

GetFailedOk returns a tuple with the Failed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFailed

`func (o *BulkMarkReadResponse) SetFailed(v []BulkMarkReadResponseFailedInner)`

SetFailed sets Failed field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


