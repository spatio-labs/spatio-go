# BulkFilesResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | **bool** |  | 
**AffectedCount** | **int32** |  | 
**FileIds** | **[]string** |  | 
**Failed** | [**[]BulkFilesResponseFailedInner**](BulkFilesResponseFailedInner.md) |  | 

## Methods

### NewBulkFilesResponse

`func NewBulkFilesResponse(success bool, affectedCount int32, fileIds []string, failed []BulkFilesResponseFailedInner, ) *BulkFilesResponse`

NewBulkFilesResponse instantiates a new BulkFilesResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBulkFilesResponseWithDefaults

`func NewBulkFilesResponseWithDefaults() *BulkFilesResponse`

NewBulkFilesResponseWithDefaults instantiates a new BulkFilesResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *BulkFilesResponse) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *BulkFilesResponse) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *BulkFilesResponse) SetSuccess(v bool)`

SetSuccess sets Success field to given value.


### GetAffectedCount

`func (o *BulkFilesResponse) GetAffectedCount() int32`

GetAffectedCount returns the AffectedCount field if non-nil, zero value otherwise.

### GetAffectedCountOk

`func (o *BulkFilesResponse) GetAffectedCountOk() (*int32, bool)`

GetAffectedCountOk returns a tuple with the AffectedCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAffectedCount

`func (o *BulkFilesResponse) SetAffectedCount(v int32)`

SetAffectedCount sets AffectedCount field to given value.


### GetFileIds

`func (o *BulkFilesResponse) GetFileIds() []string`

GetFileIds returns the FileIds field if non-nil, zero value otherwise.

### GetFileIdsOk

`func (o *BulkFilesResponse) GetFileIdsOk() (*[]string, bool)`

GetFileIdsOk returns a tuple with the FileIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileIds

`func (o *BulkFilesResponse) SetFileIds(v []string)`

SetFileIds sets FileIds field to given value.


### GetFailed

`func (o *BulkFilesResponse) GetFailed() []BulkFilesResponseFailedInner`

GetFailed returns the Failed field if non-nil, zero value otherwise.

### GetFailedOk

`func (o *BulkFilesResponse) GetFailedOk() (*[]BulkFilesResponseFailedInner, bool)`

GetFailedOk returns a tuple with the Failed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFailed

`func (o *BulkFilesResponse) SetFailed(v []BulkFilesResponseFailedInner)`

SetFailed sets Failed field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


