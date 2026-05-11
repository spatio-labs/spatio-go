# ValidateKeyBindingResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Valid** | **bool** |  | 
**Conflicts** | Pointer to **[]map[string]interface{}** |  | [optional] 

## Methods

### NewValidateKeyBindingResponse

`func NewValidateKeyBindingResponse(valid bool, ) *ValidateKeyBindingResponse`

NewValidateKeyBindingResponse instantiates a new ValidateKeyBindingResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewValidateKeyBindingResponseWithDefaults

`func NewValidateKeyBindingResponseWithDefaults() *ValidateKeyBindingResponse`

NewValidateKeyBindingResponseWithDefaults instantiates a new ValidateKeyBindingResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetValid

`func (o *ValidateKeyBindingResponse) GetValid() bool`

GetValid returns the Valid field if non-nil, zero value otherwise.

### GetValidOk

`func (o *ValidateKeyBindingResponse) GetValidOk() (*bool, bool)`

GetValidOk returns a tuple with the Valid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValid

`func (o *ValidateKeyBindingResponse) SetValid(v bool)`

SetValid sets Valid field to given value.


### GetConflicts

`func (o *ValidateKeyBindingResponse) GetConflicts() []map[string]interface{}`

GetConflicts returns the Conflicts field if non-nil, zero value otherwise.

### GetConflictsOk

`func (o *ValidateKeyBindingResponse) GetConflictsOk() (*[]map[string]interface{}, bool)`

GetConflictsOk returns a tuple with the Conflicts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConflicts

`func (o *ValidateKeyBindingResponse) SetConflicts(v []map[string]interface{})`

SetConflicts sets Conflicts field to given value.

### HasConflicts

`func (o *ValidateKeyBindingResponse) HasConflicts() bool`

HasConflicts returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


