# ExecuteChatActionResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | **bool** |  | 
**Result** | Pointer to **interface{}** | Action-specific result payload. | [optional] 

## Methods

### NewExecuteChatActionResponse

`func NewExecuteChatActionResponse(success bool, ) *ExecuteChatActionResponse`

NewExecuteChatActionResponse instantiates a new ExecuteChatActionResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewExecuteChatActionResponseWithDefaults

`func NewExecuteChatActionResponseWithDefaults() *ExecuteChatActionResponse`

NewExecuteChatActionResponseWithDefaults instantiates a new ExecuteChatActionResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *ExecuteChatActionResponse) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *ExecuteChatActionResponse) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *ExecuteChatActionResponse) SetSuccess(v bool)`

SetSuccess sets Success field to given value.


### GetResult

`func (o *ExecuteChatActionResponse) GetResult() interface{}`

GetResult returns the Result field if non-nil, zero value otherwise.

### GetResultOk

`func (o *ExecuteChatActionResponse) GetResultOk() (*interface{}, bool)`

GetResultOk returns a tuple with the Result field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResult

`func (o *ExecuteChatActionResponse) SetResult(v interface{})`

SetResult sets Result field to given value.

### HasResult

`func (o *ExecuteChatActionResponse) HasResult() bool`

HasResult returns a boolean if a field has been set.

### SetResultNil

`func (o *ExecuteChatActionResponse) SetResultNil(b bool)`

 SetResultNil sets the value for Result to be an explicit nil

### UnsetResult
`func (o *ExecuteChatActionResponse) UnsetResult()`

UnsetResult ensures that no value is present for Result, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


