# BulkArchiveResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | **bool** | &#x60;true&#x60; only when zero rows in &#x60;failed&#x60;. | 
**Archived** | **[]string** |  | 
**Failed** | [**[]BulkArchiveResponseFailedInner**](BulkArchiveResponseFailedInner.md) |  | 

## Methods

### NewBulkArchiveResponse

`func NewBulkArchiveResponse(success bool, archived []string, failed []BulkArchiveResponseFailedInner, ) *BulkArchiveResponse`

NewBulkArchiveResponse instantiates a new BulkArchiveResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBulkArchiveResponseWithDefaults

`func NewBulkArchiveResponseWithDefaults() *BulkArchiveResponse`

NewBulkArchiveResponseWithDefaults instantiates a new BulkArchiveResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *BulkArchiveResponse) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *BulkArchiveResponse) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *BulkArchiveResponse) SetSuccess(v bool)`

SetSuccess sets Success field to given value.


### GetArchived

`func (o *BulkArchiveResponse) GetArchived() []string`

GetArchived returns the Archived field if non-nil, zero value otherwise.

### GetArchivedOk

`func (o *BulkArchiveResponse) GetArchivedOk() (*[]string, bool)`

GetArchivedOk returns a tuple with the Archived field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchived

`func (o *BulkArchiveResponse) SetArchived(v []string)`

SetArchived sets Archived field to given value.


### GetFailed

`func (o *BulkArchiveResponse) GetFailed() []BulkArchiveResponseFailedInner`

GetFailed returns the Failed field if non-nil, zero value otherwise.

### GetFailedOk

`func (o *BulkArchiveResponse) GetFailedOk() (*[]BulkArchiveResponseFailedInner, bool)`

GetFailedOk returns a tuple with the Failed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFailed

`func (o *BulkArchiveResponse) SetFailed(v []BulkArchiveResponseFailedInner)`

SetFailed sets Failed field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


