# BulkUpdateTasksRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TaskIds** | **[]string** |  | 
**AccountIds** | Pointer to **[]string** |  | [optional] 
**AccountId** | Pointer to **string** |  | [optional] 
**Updates** | [**UpdateTaskRequest**](UpdateTaskRequest.md) |  | 

## Methods

### NewBulkUpdateTasksRequest

`func NewBulkUpdateTasksRequest(taskIds []string, updates UpdateTaskRequest, ) *BulkUpdateTasksRequest`

NewBulkUpdateTasksRequest instantiates a new BulkUpdateTasksRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBulkUpdateTasksRequestWithDefaults

`func NewBulkUpdateTasksRequestWithDefaults() *BulkUpdateTasksRequest`

NewBulkUpdateTasksRequestWithDefaults instantiates a new BulkUpdateTasksRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTaskIds

`func (o *BulkUpdateTasksRequest) GetTaskIds() []string`

GetTaskIds returns the TaskIds field if non-nil, zero value otherwise.

### GetTaskIdsOk

`func (o *BulkUpdateTasksRequest) GetTaskIdsOk() (*[]string, bool)`

GetTaskIdsOk returns a tuple with the TaskIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaskIds

`func (o *BulkUpdateTasksRequest) SetTaskIds(v []string)`

SetTaskIds sets TaskIds field to given value.


### GetAccountIds

`func (o *BulkUpdateTasksRequest) GetAccountIds() []string`

GetAccountIds returns the AccountIds field if non-nil, zero value otherwise.

### GetAccountIdsOk

`func (o *BulkUpdateTasksRequest) GetAccountIdsOk() (*[]string, bool)`

GetAccountIdsOk returns a tuple with the AccountIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountIds

`func (o *BulkUpdateTasksRequest) SetAccountIds(v []string)`

SetAccountIds sets AccountIds field to given value.

### HasAccountIds

`func (o *BulkUpdateTasksRequest) HasAccountIds() bool`

HasAccountIds returns a boolean if a field has been set.

### GetAccountId

`func (o *BulkUpdateTasksRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *BulkUpdateTasksRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *BulkUpdateTasksRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *BulkUpdateTasksRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetUpdates

`func (o *BulkUpdateTasksRequest) GetUpdates() UpdateTaskRequest`

GetUpdates returns the Updates field if non-nil, zero value otherwise.

### GetUpdatesOk

`func (o *BulkUpdateTasksRequest) GetUpdatesOk() (*UpdateTaskRequest, bool)`

GetUpdatesOk returns a tuple with the Updates field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdates

`func (o *BulkUpdateTasksRequest) SetUpdates(v UpdateTaskRequest)`

SetUpdates sets Updates field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


