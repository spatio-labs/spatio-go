# BulkUpdateTasksResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | **bool** |  | 
**AffectedCount** | **int32** |  | 
**Tasks** | [**[]Task**](Task.md) |  | 
**Failed** | [**[]BulkDeleteTasksResponseFailedInner**](BulkDeleteTasksResponseFailedInner.md) |  | 

## Methods

### NewBulkUpdateTasksResponse

`func NewBulkUpdateTasksResponse(success bool, affectedCount int32, tasks []Task, failed []BulkDeleteTasksResponseFailedInner, ) *BulkUpdateTasksResponse`

NewBulkUpdateTasksResponse instantiates a new BulkUpdateTasksResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBulkUpdateTasksResponseWithDefaults

`func NewBulkUpdateTasksResponseWithDefaults() *BulkUpdateTasksResponse`

NewBulkUpdateTasksResponseWithDefaults instantiates a new BulkUpdateTasksResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *BulkUpdateTasksResponse) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *BulkUpdateTasksResponse) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *BulkUpdateTasksResponse) SetSuccess(v bool)`

SetSuccess sets Success field to given value.


### GetAffectedCount

`func (o *BulkUpdateTasksResponse) GetAffectedCount() int32`

GetAffectedCount returns the AffectedCount field if non-nil, zero value otherwise.

### GetAffectedCountOk

`func (o *BulkUpdateTasksResponse) GetAffectedCountOk() (*int32, bool)`

GetAffectedCountOk returns a tuple with the AffectedCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAffectedCount

`func (o *BulkUpdateTasksResponse) SetAffectedCount(v int32)`

SetAffectedCount sets AffectedCount field to given value.


### GetTasks

`func (o *BulkUpdateTasksResponse) GetTasks() []Task`

GetTasks returns the Tasks field if non-nil, zero value otherwise.

### GetTasksOk

`func (o *BulkUpdateTasksResponse) GetTasksOk() (*[]Task, bool)`

GetTasksOk returns a tuple with the Tasks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTasks

`func (o *BulkUpdateTasksResponse) SetTasks(v []Task)`

SetTasks sets Tasks field to given value.


### GetFailed

`func (o *BulkUpdateTasksResponse) GetFailed() []BulkDeleteTasksResponseFailedInner`

GetFailed returns the Failed field if non-nil, zero value otherwise.

### GetFailedOk

`func (o *BulkUpdateTasksResponse) GetFailedOk() (*[]BulkDeleteTasksResponseFailedInner, bool)`

GetFailedOk returns a tuple with the Failed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFailed

`func (o *BulkUpdateTasksResponse) SetFailed(v []BulkDeleteTasksResponseFailedInner)`

SetFailed sets Failed field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


