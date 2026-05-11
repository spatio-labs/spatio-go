# UpdateKeyBindingRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Key** | **string** |  | 
**Modifiers** | Pointer to **[]string** |  | [optional] 

## Methods

### NewUpdateKeyBindingRequest

`func NewUpdateKeyBindingRequest(key string, ) *UpdateKeyBindingRequest`

NewUpdateKeyBindingRequest instantiates a new UpdateKeyBindingRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateKeyBindingRequestWithDefaults

`func NewUpdateKeyBindingRequestWithDefaults() *UpdateKeyBindingRequest`

NewUpdateKeyBindingRequestWithDefaults instantiates a new UpdateKeyBindingRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetKey

`func (o *UpdateKeyBindingRequest) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *UpdateKeyBindingRequest) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *UpdateKeyBindingRequest) SetKey(v string)`

SetKey sets Key field to given value.


### GetModifiers

`func (o *UpdateKeyBindingRequest) GetModifiers() []string`

GetModifiers returns the Modifiers field if non-nil, zero value otherwise.

### GetModifiersOk

`func (o *UpdateKeyBindingRequest) GetModifiersOk() (*[]string, bool)`

GetModifiersOk returns a tuple with the Modifiers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModifiers

`func (o *UpdateKeyBindingRequest) SetModifiers(v []string)`

SetModifiers sets Modifiers field to given value.

### HasModifiers

`func (o *UpdateKeyBindingRequest) HasModifiers() bool`

HasModifiers returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


