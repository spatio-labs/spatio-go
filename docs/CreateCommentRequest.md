# CreateCommentRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Body** | Pointer to **string** |  | [optional] 
**Content** | Pointer to **string** |  | [optional] 
**ParentCommentId** | Pointer to **NullableString** |  | [optional] 
**BlockId** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewCreateCommentRequest

`func NewCreateCommentRequest() *CreateCommentRequest`

NewCreateCommentRequest instantiates a new CreateCommentRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateCommentRequestWithDefaults

`func NewCreateCommentRequestWithDefaults() *CreateCommentRequest`

NewCreateCommentRequestWithDefaults instantiates a new CreateCommentRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBody

`func (o *CreateCommentRequest) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *CreateCommentRequest) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *CreateCommentRequest) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *CreateCommentRequest) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetContent

`func (o *CreateCommentRequest) GetContent() string`

GetContent returns the Content field if non-nil, zero value otherwise.

### GetContentOk

`func (o *CreateCommentRequest) GetContentOk() (*string, bool)`

GetContentOk returns a tuple with the Content field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContent

`func (o *CreateCommentRequest) SetContent(v string)`

SetContent sets Content field to given value.

### HasContent

`func (o *CreateCommentRequest) HasContent() bool`

HasContent returns a boolean if a field has been set.

### GetParentCommentId

`func (o *CreateCommentRequest) GetParentCommentId() string`

GetParentCommentId returns the ParentCommentId field if non-nil, zero value otherwise.

### GetParentCommentIdOk

`func (o *CreateCommentRequest) GetParentCommentIdOk() (*string, bool)`

GetParentCommentIdOk returns a tuple with the ParentCommentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParentCommentId

`func (o *CreateCommentRequest) SetParentCommentId(v string)`

SetParentCommentId sets ParentCommentId field to given value.

### HasParentCommentId

`func (o *CreateCommentRequest) HasParentCommentId() bool`

HasParentCommentId returns a boolean if a field has been set.

### SetParentCommentIdNil

`func (o *CreateCommentRequest) SetParentCommentIdNil(b bool)`

 SetParentCommentIdNil sets the value for ParentCommentId to be an explicit nil

### UnsetParentCommentId
`func (o *CreateCommentRequest) UnsetParentCommentId()`

UnsetParentCommentId ensures that no value is present for ParentCommentId, not even an explicit nil
### GetBlockId

`func (o *CreateCommentRequest) GetBlockId() string`

GetBlockId returns the BlockId field if non-nil, zero value otherwise.

### GetBlockIdOk

`func (o *CreateCommentRequest) GetBlockIdOk() (*string, bool)`

GetBlockIdOk returns a tuple with the BlockId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlockId

`func (o *CreateCommentRequest) SetBlockId(v string)`

SetBlockId sets BlockId field to given value.

### HasBlockId

`func (o *CreateCommentRequest) HasBlockId() bool`

HasBlockId returns a boolean if a field has been set.

### SetBlockIdNil

`func (o *CreateCommentRequest) SetBlockIdNil(b bool)`

 SetBlockIdNil sets the value for BlockId to be an explicit nil

### UnsetBlockId
`func (o *CreateCommentRequest) UnsetBlockId()`

UnsetBlockId ensures that no value is present for BlockId, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


