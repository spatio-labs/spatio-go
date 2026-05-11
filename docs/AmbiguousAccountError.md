# AmbiguousAccountError

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Error** | **string** | Human-readable error message. | 
**Code** | Pointer to **string** | Machine-readable error code. Stable across releases for the canonical codes (&#x60;ambiguous_account&#x60;, &#x60;no_notes_provider&#x60;, &#x60;note_not_found&#x60;). Absent for generic errors.  | [optional] 
**Accounts** | Pointer to [**[]AccountChoice**](AccountChoice.md) |  | [optional] 

## Methods

### NewAmbiguousAccountError

`func NewAmbiguousAccountError(error_ string, ) *AmbiguousAccountError`

NewAmbiguousAccountError instantiates a new AmbiguousAccountError object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAmbiguousAccountErrorWithDefaults

`func NewAmbiguousAccountErrorWithDefaults() *AmbiguousAccountError`

NewAmbiguousAccountErrorWithDefaults instantiates a new AmbiguousAccountError object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetError

`func (o *AmbiguousAccountError) GetError() string`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *AmbiguousAccountError) GetErrorOk() (*string, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *AmbiguousAccountError) SetError(v string)`

SetError sets Error field to given value.


### GetCode

`func (o *AmbiguousAccountError) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *AmbiguousAccountError) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *AmbiguousAccountError) SetCode(v string)`

SetCode sets Code field to given value.

### HasCode

`func (o *AmbiguousAccountError) HasCode() bool`

HasCode returns a boolean if a field has been set.

### GetAccounts

`func (o *AmbiguousAccountError) GetAccounts() []AccountChoice`

GetAccounts returns the Accounts field if non-nil, zero value otherwise.

### GetAccountsOk

`func (o *AmbiguousAccountError) GetAccountsOk() (*[]AccountChoice, bool)`

GetAccountsOk returns a tuple with the Accounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccounts

`func (o *AmbiguousAccountError) SetAccounts(v []AccountChoice)`

SetAccounts sets Accounts field to given value.

### HasAccounts

`func (o *AmbiguousAccountError) HasAccounts() bool`

HasAccounts returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


