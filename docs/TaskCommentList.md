# TaskCommentList

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Comments** | [**[]TaskComment**](TaskComment.md) |  | 
**Total** | **int32** |  | 

## Methods

### NewTaskCommentList

`func NewTaskCommentList(comments []TaskComment, total int32, ) *TaskCommentList`

NewTaskCommentList instantiates a new TaskCommentList object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTaskCommentListWithDefaults

`func NewTaskCommentListWithDefaults() *TaskCommentList`

NewTaskCommentListWithDefaults instantiates a new TaskCommentList object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetComments

`func (o *TaskCommentList) GetComments() []TaskComment`

GetComments returns the Comments field if non-nil, zero value otherwise.

### GetCommentsOk

`func (o *TaskCommentList) GetCommentsOk() (*[]TaskComment, bool)`

GetCommentsOk returns a tuple with the Comments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetComments

`func (o *TaskCommentList) SetComments(v []TaskComment)`

SetComments sets Comments field to given value.


### GetTotal

`func (o *TaskCommentList) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *TaskCommentList) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *TaskCommentList) SetTotal(v int32)`

SetTotal sets Total field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


