# EnableShareRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**SetPassword** | Pointer to **bool** |  | [optional] 
**Password** | Pointer to **string** |  | [optional] 

## Methods

### NewEnableShareRequest

`func NewEnableShareRequest() *EnableShareRequest`

NewEnableShareRequest instantiates a new EnableShareRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEnableShareRequestWithDefaults

`func NewEnableShareRequestWithDefaults() *EnableShareRequest`

NewEnableShareRequestWithDefaults instantiates a new EnableShareRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSetPassword

`func (o *EnableShareRequest) GetSetPassword() bool`

GetSetPassword returns the SetPassword field if non-nil, zero value otherwise.

### GetSetPasswordOk

`func (o *EnableShareRequest) GetSetPasswordOk() (*bool, bool)`

GetSetPasswordOk returns a tuple with the SetPassword field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSetPassword

`func (o *EnableShareRequest) SetSetPassword(v bool)`

SetSetPassword sets SetPassword field to given value.

### HasSetPassword

`func (o *EnableShareRequest) HasSetPassword() bool`

HasSetPassword returns a boolean if a field has been set.

### GetPassword

`func (o *EnableShareRequest) GetPassword() string`

GetPassword returns the Password field if non-nil, zero value otherwise.

### GetPasswordOk

`func (o *EnableShareRequest) GetPasswordOk() (*string, bool)`

GetPasswordOk returns a tuple with the Password field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPassword

`func (o *EnableShareRequest) SetPassword(v string)`

SetPassword sets Password field to given value.

### HasPassword

`func (o *EnableShareRequest) HasPassword() bool`

HasPassword returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


