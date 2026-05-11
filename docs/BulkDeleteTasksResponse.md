# BulkDeleteTasksResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | **bool** |  | 
**AffectedCount** | **int32** |  | 
**TaskIds** | **[]string** |  | 
**Failed** | [**[]BulkDeleteTasksResponseFailedInner**](BulkDeleteTasksResponseFailedInner.md) |  | 

## Methods

### NewBulkDeleteTasksResponse

`func NewBulkDeleteTasksResponse(success bool, affectedCount int32, taskIds []string, failed []BulkDeleteTasksResponseFailedInner, ) *BulkDeleteTasksResponse`

NewBulkDeleteTasksResponse instantiates a new BulkDeleteTasksResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBulkDeleteTasksResponseWithDefaults

`func NewBulkDeleteTasksResponseWithDefaults() *BulkDeleteTasksResponse`

NewBulkDeleteTasksResponseWithDefaults instantiates a new BulkDeleteTasksResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *BulkDeleteTasksResponse) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *BulkDeleteTasksResponse) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *BulkDeleteTasksResponse) SetSuccess(v bool)`

SetSuccess sets Success field to given value.


### GetAffectedCount

`func (o *BulkDeleteTasksResponse) GetAffectedCount() int32`

GetAffectedCount returns the AffectedCount field if non-nil, zero value otherwise.

### GetAffectedCountOk

`func (o *BulkDeleteTasksResponse) GetAffectedCountOk() (*int32, bool)`

GetAffectedCountOk returns a tuple with the AffectedCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAffectedCount

`func (o *BulkDeleteTasksResponse) SetAffectedCount(v int32)`

SetAffectedCount sets AffectedCount field to given value.


### GetTaskIds

`func (o *BulkDeleteTasksResponse) GetTaskIds() []string`

GetTaskIds returns the TaskIds field if non-nil, zero value otherwise.

### GetTaskIdsOk

`func (o *BulkDeleteTasksResponse) GetTaskIdsOk() (*[]string, bool)`

GetTaskIdsOk returns a tuple with the TaskIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaskIds

`func (o *BulkDeleteTasksResponse) SetTaskIds(v []string)`

SetTaskIds sets TaskIds field to given value.


### GetFailed

`func (o *BulkDeleteTasksResponse) GetFailed() []BulkDeleteTasksResponseFailedInner`

GetFailed returns the Failed field if non-nil, zero value otherwise.

### GetFailedOk

`func (o *BulkDeleteTasksResponse) GetFailedOk() (*[]BulkDeleteTasksResponseFailedInner, bool)`

GetFailedOk returns a tuple with the Failed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFailed

`func (o *BulkDeleteTasksResponse) SetFailed(v []BulkDeleteTasksResponseFailedInner)`

SetFailed sets Failed field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


