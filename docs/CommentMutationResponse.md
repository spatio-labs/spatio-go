# CommentMutationResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Comment** | [**Comment**](Comment.md) |  | 
**Success** | **bool** |  | 

## Methods

### NewCommentMutationResponse

`func NewCommentMutationResponse(comment Comment, success bool, ) *CommentMutationResponse`

NewCommentMutationResponse instantiates a new CommentMutationResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCommentMutationResponseWithDefaults

`func NewCommentMutationResponseWithDefaults() *CommentMutationResponse`

NewCommentMutationResponseWithDefaults instantiates a new CommentMutationResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetComment

`func (o *CommentMutationResponse) GetComment() Comment`

GetComment returns the Comment field if non-nil, zero value otherwise.

### GetCommentOk

`func (o *CommentMutationResponse) GetCommentOk() (*Comment, bool)`

GetCommentOk returns a tuple with the Comment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetComment

`func (o *CommentMutationResponse) SetComment(v Comment)`

SetComment sets Comment field to given value.


### GetSuccess

`func (o *CommentMutationResponse) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *CommentMutationResponse) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *CommentMutationResponse) SetSuccess(v bool)`

SetSuccess sets Success field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


