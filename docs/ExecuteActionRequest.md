# ExecuteActionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ActionId** | **string** |  | 
**Params** | Pointer to **map[string]interface{}** |  | [optional] 
**AccountId** | Pointer to **string** |  | [optional] 

## Methods

### NewExecuteActionRequest

`func NewExecuteActionRequest(actionId string, ) *ExecuteActionRequest`

NewExecuteActionRequest instantiates a new ExecuteActionRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewExecuteActionRequestWithDefaults

`func NewExecuteActionRequestWithDefaults() *ExecuteActionRequest`

NewExecuteActionRequestWithDefaults instantiates a new ExecuteActionRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetActionId

`func (o *ExecuteActionRequest) GetActionId() string`

GetActionId returns the ActionId field if non-nil, zero value otherwise.

### GetActionIdOk

`func (o *ExecuteActionRequest) GetActionIdOk() (*string, bool)`

GetActionIdOk returns a tuple with the ActionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionId

`func (o *ExecuteActionRequest) SetActionId(v string)`

SetActionId sets ActionId field to given value.


### GetParams

`func (o *ExecuteActionRequest) GetParams() map[string]interface{}`

GetParams returns the Params field if non-nil, zero value otherwise.

### GetParamsOk

`func (o *ExecuteActionRequest) GetParamsOk() (*map[string]interface{}, bool)`

GetParamsOk returns a tuple with the Params field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParams

`func (o *ExecuteActionRequest) SetParams(v map[string]interface{})`

SetParams sets Params field to given value.

### HasParams

`func (o *ExecuteActionRequest) HasParams() bool`

HasParams returns a boolean if a field has been set.

### GetAccountId

`func (o *ExecuteActionRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *ExecuteActionRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *ExecuteActionRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *ExecuteActionRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


