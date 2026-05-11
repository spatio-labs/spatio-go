# BulkDeleteEmailsResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | **bool** |  | 
**Deleted** | **[]string** |  | 
**Failed** | [**[]BulkArchiveResponseFailedInner**](BulkArchiveResponseFailedInner.md) |  | 

## Methods

### NewBulkDeleteEmailsResponse

`func NewBulkDeleteEmailsResponse(success bool, deleted []string, failed []BulkArchiveResponseFailedInner, ) *BulkDeleteEmailsResponse`

NewBulkDeleteEmailsResponse instantiates a new BulkDeleteEmailsResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBulkDeleteEmailsResponseWithDefaults

`func NewBulkDeleteEmailsResponseWithDefaults() *BulkDeleteEmailsResponse`

NewBulkDeleteEmailsResponseWithDefaults instantiates a new BulkDeleteEmailsResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *BulkDeleteEmailsResponse) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *BulkDeleteEmailsResponse) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *BulkDeleteEmailsResponse) SetSuccess(v bool)`

SetSuccess sets Success field to given value.


### GetDeleted

`func (o *BulkDeleteEmailsResponse) GetDeleted() []string`

GetDeleted returns the Deleted field if non-nil, zero value otherwise.

### GetDeletedOk

`func (o *BulkDeleteEmailsResponse) GetDeletedOk() (*[]string, bool)`

GetDeletedOk returns a tuple with the Deleted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeleted

`func (o *BulkDeleteEmailsResponse) SetDeleted(v []string)`

SetDeleted sets Deleted field to given value.


### GetFailed

`func (o *BulkDeleteEmailsResponse) GetFailed() []BulkArchiveResponseFailedInner`

GetFailed returns the Failed field if non-nil, zero value otherwise.

### GetFailedOk

`func (o *BulkDeleteEmailsResponse) GetFailedOk() (*[]BulkArchiveResponseFailedInner, bool)`

GetFailedOk returns a tuple with the Failed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFailed

`func (o *BulkDeleteEmailsResponse) SetFailed(v []BulkArchiveResponseFailedInner)`

SetFailed sets Failed field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


