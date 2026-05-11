# PasswordRequiredError

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Error** | **string** | Human-readable error message. | 
**Code** | Pointer to **string** | Machine-readable error code. Stable across releases for the canonical codes (&#x60;ambiguous_account&#x60;, &#x60;no_notes_provider&#x60;, &#x60;note_not_found&#x60;). Absent for generic errors.  | [optional] 
**RequiresPassword** | **bool** |  | 
**InvalidPassword** | Pointer to **bool** |  | [optional] 

## Methods

### NewPasswordRequiredError

`func NewPasswordRequiredError(error_ string, requiresPassword bool, ) *PasswordRequiredError`

NewPasswordRequiredError instantiates a new PasswordRequiredError object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPasswordRequiredErrorWithDefaults

`func NewPasswordRequiredErrorWithDefaults() *PasswordRequiredError`

NewPasswordRequiredErrorWithDefaults instantiates a new PasswordRequiredError object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetError

`func (o *PasswordRequiredError) GetError() string`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *PasswordRequiredError) GetErrorOk() (*string, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *PasswordRequiredError) SetError(v string)`

SetError sets Error field to given value.


### GetCode

`func (o *PasswordRequiredError) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *PasswordRequiredError) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *PasswordRequiredError) SetCode(v string)`

SetCode sets Code field to given value.

### HasCode

`func (o *PasswordRequiredError) HasCode() bool`

HasCode returns a boolean if a field has been set.

### GetRequiresPassword

`func (o *PasswordRequiredError) GetRequiresPassword() bool`

GetRequiresPassword returns the RequiresPassword field if non-nil, zero value otherwise.

### GetRequiresPasswordOk

`func (o *PasswordRequiredError) GetRequiresPasswordOk() (*bool, bool)`

GetRequiresPasswordOk returns a tuple with the RequiresPassword field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequiresPassword

`func (o *PasswordRequiredError) SetRequiresPassword(v bool)`

SetRequiresPassword sets RequiresPassword field to given value.


### GetInvalidPassword

`func (o *PasswordRequiredError) GetInvalidPassword() bool`

GetInvalidPassword returns the InvalidPassword field if non-nil, zero value otherwise.

### GetInvalidPasswordOk

`func (o *PasswordRequiredError) GetInvalidPasswordOk() (*bool, bool)`

GetInvalidPasswordOk returns a tuple with the InvalidPassword field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInvalidPassword

`func (o *PasswordRequiredError) SetInvalidPassword(v bool)`

SetInvalidPassword sets InvalidPassword field to given value.

### HasInvalidPassword

`func (o *PasswordRequiredError) HasInvalidPassword() bool`

HasInvalidPassword returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


