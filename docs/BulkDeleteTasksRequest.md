# BulkDeleteTasksRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TaskIds** | Pointer to **[]string** |  | [optional] 
**AccountIds** | Pointer to **[]string** | Parallel slice with taskIds — accountIds[i] targets taskIds[i]. | [optional] 
**TaskId** | Pointer to **string** | Singular fallback when only deleting one task. | [optional] 
**AccountId** | Pointer to **string** |  | [optional] 

## Methods

### NewBulkDeleteTasksRequest

`func NewBulkDeleteTasksRequest() *BulkDeleteTasksRequest`

NewBulkDeleteTasksRequest instantiates a new BulkDeleteTasksRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBulkDeleteTasksRequestWithDefaults

`func NewBulkDeleteTasksRequestWithDefaults() *BulkDeleteTasksRequest`

NewBulkDeleteTasksRequestWithDefaults instantiates a new BulkDeleteTasksRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTaskIds

`func (o *BulkDeleteTasksRequest) GetTaskIds() []string`

GetTaskIds returns the TaskIds field if non-nil, zero value otherwise.

### GetTaskIdsOk

`func (o *BulkDeleteTasksRequest) GetTaskIdsOk() (*[]string, bool)`

GetTaskIdsOk returns a tuple with the TaskIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaskIds

`func (o *BulkDeleteTasksRequest) SetTaskIds(v []string)`

SetTaskIds sets TaskIds field to given value.

### HasTaskIds

`func (o *BulkDeleteTasksRequest) HasTaskIds() bool`

HasTaskIds returns a boolean if a field has been set.

### GetAccountIds

`func (o *BulkDeleteTasksRequest) GetAccountIds() []string`

GetAccountIds returns the AccountIds field if non-nil, zero value otherwise.

### GetAccountIdsOk

`func (o *BulkDeleteTasksRequest) GetAccountIdsOk() (*[]string, bool)`

GetAccountIdsOk returns a tuple with the AccountIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountIds

`func (o *BulkDeleteTasksRequest) SetAccountIds(v []string)`

SetAccountIds sets AccountIds field to given value.

### HasAccountIds

`func (o *BulkDeleteTasksRequest) HasAccountIds() bool`

HasAccountIds returns a boolean if a field has been set.

### GetTaskId

`func (o *BulkDeleteTasksRequest) GetTaskId() string`

GetTaskId returns the TaskId field if non-nil, zero value otherwise.

### GetTaskIdOk

`func (o *BulkDeleteTasksRequest) GetTaskIdOk() (*string, bool)`

GetTaskIdOk returns a tuple with the TaskId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaskId

`func (o *BulkDeleteTasksRequest) SetTaskId(v string)`

SetTaskId sets TaskId field to given value.

### HasTaskId

`func (o *BulkDeleteTasksRequest) HasTaskId() bool`

HasTaskId returns a boolean if a field has been set.

### GetAccountId

`func (o *BulkDeleteTasksRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *BulkDeleteTasksRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *BulkDeleteTasksRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *BulkDeleteTasksRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


