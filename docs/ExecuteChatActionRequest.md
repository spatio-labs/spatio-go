# ExecuteChatActionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ActionId** | **string** |  | 
**Params** | Pointer to **interface{}** | Action-specific parameters. Free-form because the shape depends on &#x60;action_id&#x60;. See &#x60;GET /actions&#x60; for the per-id contract.  | [optional] 

## Methods

### NewExecuteChatActionRequest

`func NewExecuteChatActionRequest(actionId string, ) *ExecuteChatActionRequest`

NewExecuteChatActionRequest instantiates a new ExecuteChatActionRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewExecuteChatActionRequestWithDefaults

`func NewExecuteChatActionRequestWithDefaults() *ExecuteChatActionRequest`

NewExecuteChatActionRequestWithDefaults instantiates a new ExecuteChatActionRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetActionId

`func (o *ExecuteChatActionRequest) GetActionId() string`

GetActionId returns the ActionId field if non-nil, zero value otherwise.

### GetActionIdOk

`func (o *ExecuteChatActionRequest) GetActionIdOk() (*string, bool)`

GetActionIdOk returns a tuple with the ActionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionId

`func (o *ExecuteChatActionRequest) SetActionId(v string)`

SetActionId sets ActionId field to given value.


### GetParams

`func (o *ExecuteChatActionRequest) GetParams() interface{}`

GetParams returns the Params field if non-nil, zero value otherwise.

### GetParamsOk

`func (o *ExecuteChatActionRequest) GetParamsOk() (*interface{}, bool)`

GetParamsOk returns a tuple with the Params field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParams

`func (o *ExecuteChatActionRequest) SetParams(v interface{})`

SetParams sets Params field to given value.

### HasParams

`func (o *ExecuteChatActionRequest) HasParams() bool`

HasParams returns a boolean if a field has been set.

### SetParamsNil

`func (o *ExecuteChatActionRequest) SetParamsNil(b bool)`

 SetParamsNil sets the value for Params to be an explicit nil

### UnsetParams
`func (o *ExecuteChatActionRequest) UnsetParams()`

UnsetParams ensures that no value is present for Params, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


