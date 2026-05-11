# QuotaExceededError

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Error** | **string** | Human-readable error message. | 
**Code** | Pointer to **string** | Machine-readable error code. Stable across releases for the canonical codes (&#x60;ambiguous_account&#x60;, &#x60;no_notes_provider&#x60;, &#x60;note_not_found&#x60;). Absent for generic errors.  | [optional] 

## Methods

### NewQuotaExceededError

`func NewQuotaExceededError(error_ string, ) *QuotaExceededError`

NewQuotaExceededError instantiates a new QuotaExceededError object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewQuotaExceededErrorWithDefaults

`func NewQuotaExceededErrorWithDefaults() *QuotaExceededError`

NewQuotaExceededErrorWithDefaults instantiates a new QuotaExceededError object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetError

`func (o *QuotaExceededError) GetError() string`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *QuotaExceededError) GetErrorOk() (*string, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *QuotaExceededError) SetError(v string)`

SetError sets Error field to given value.


### GetCode

`func (o *QuotaExceededError) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *QuotaExceededError) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *QuotaExceededError) SetCode(v string)`

SetCode sets Code field to given value.

### HasCode

`func (o *QuotaExceededError) HasCode() bool`

HasCode returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


