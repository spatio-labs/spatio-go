# ValidateKeyBindingRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ActionId** | **string** |  | 
**Key** | **string** |  | 
**Modifiers** | Pointer to **[]string** |  | [optional] 

## Methods

### NewValidateKeyBindingRequest

`func NewValidateKeyBindingRequest(actionId string, key string, ) *ValidateKeyBindingRequest`

NewValidateKeyBindingRequest instantiates a new ValidateKeyBindingRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewValidateKeyBindingRequestWithDefaults

`func NewValidateKeyBindingRequestWithDefaults() *ValidateKeyBindingRequest`

NewValidateKeyBindingRequestWithDefaults instantiates a new ValidateKeyBindingRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetActionId

`func (o *ValidateKeyBindingRequest) GetActionId() string`

GetActionId returns the ActionId field if non-nil, zero value otherwise.

### GetActionIdOk

`func (o *ValidateKeyBindingRequest) GetActionIdOk() (*string, bool)`

GetActionIdOk returns a tuple with the ActionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionId

`func (o *ValidateKeyBindingRequest) SetActionId(v string)`

SetActionId sets ActionId field to given value.


### GetKey

`func (o *ValidateKeyBindingRequest) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *ValidateKeyBindingRequest) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *ValidateKeyBindingRequest) SetKey(v string)`

SetKey sets Key field to given value.


### GetModifiers

`func (o *ValidateKeyBindingRequest) GetModifiers() []string`

GetModifiers returns the Modifiers field if non-nil, zero value otherwise.

### GetModifiersOk

`func (o *ValidateKeyBindingRequest) GetModifiersOk() (*[]string, bool)`

GetModifiersOk returns a tuple with the Modifiers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModifiers

`func (o *ValidateKeyBindingRequest) SetModifiers(v []string)`

SetModifiers sets Modifiers field to given value.

### HasModifiers

`func (o *ValidateKeyBindingRequest) HasModifiers() bool`

HasModifiers returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


