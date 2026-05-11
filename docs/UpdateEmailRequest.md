# UpdateEmailRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccountId** | Pointer to **string** |  | [optional] 
**IsRead** | Pointer to **bool** |  | [optional] 
**IsStarred** | Pointer to **bool** |  | [optional] 
**AddLabels** | Pointer to **[]string** |  | [optional] 
**RemoveLabels** | Pointer to **[]string** |  | [optional] 

## Methods

### NewUpdateEmailRequest

`func NewUpdateEmailRequest() *UpdateEmailRequest`

NewUpdateEmailRequest instantiates a new UpdateEmailRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateEmailRequestWithDefaults

`func NewUpdateEmailRequestWithDefaults() *UpdateEmailRequest`

NewUpdateEmailRequestWithDefaults instantiates a new UpdateEmailRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccountId

`func (o *UpdateEmailRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *UpdateEmailRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *UpdateEmailRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *UpdateEmailRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetIsRead

`func (o *UpdateEmailRequest) GetIsRead() bool`

GetIsRead returns the IsRead field if non-nil, zero value otherwise.

### GetIsReadOk

`func (o *UpdateEmailRequest) GetIsReadOk() (*bool, bool)`

GetIsReadOk returns a tuple with the IsRead field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsRead

`func (o *UpdateEmailRequest) SetIsRead(v bool)`

SetIsRead sets IsRead field to given value.

### HasIsRead

`func (o *UpdateEmailRequest) HasIsRead() bool`

HasIsRead returns a boolean if a field has been set.

### GetIsStarred

`func (o *UpdateEmailRequest) GetIsStarred() bool`

GetIsStarred returns the IsStarred field if non-nil, zero value otherwise.

### GetIsStarredOk

`func (o *UpdateEmailRequest) GetIsStarredOk() (*bool, bool)`

GetIsStarredOk returns a tuple with the IsStarred field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsStarred

`func (o *UpdateEmailRequest) SetIsStarred(v bool)`

SetIsStarred sets IsStarred field to given value.

### HasIsStarred

`func (o *UpdateEmailRequest) HasIsStarred() bool`

HasIsStarred returns a boolean if a field has been set.

### GetAddLabels

`func (o *UpdateEmailRequest) GetAddLabels() []string`

GetAddLabels returns the AddLabels field if non-nil, zero value otherwise.

### GetAddLabelsOk

`func (o *UpdateEmailRequest) GetAddLabelsOk() (*[]string, bool)`

GetAddLabelsOk returns a tuple with the AddLabels field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddLabels

`func (o *UpdateEmailRequest) SetAddLabels(v []string)`

SetAddLabels sets AddLabels field to given value.

### HasAddLabels

`func (o *UpdateEmailRequest) HasAddLabels() bool`

HasAddLabels returns a boolean if a field has been set.

### GetRemoveLabels

`func (o *UpdateEmailRequest) GetRemoveLabels() []string`

GetRemoveLabels returns the RemoveLabels field if non-nil, zero value otherwise.

### GetRemoveLabelsOk

`func (o *UpdateEmailRequest) GetRemoveLabelsOk() (*[]string, bool)`

GetRemoveLabelsOk returns a tuple with the RemoveLabels field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRemoveLabels

`func (o *UpdateEmailRequest) SetRemoveLabels(v []string)`

SetRemoveLabels sets RemoveLabels field to given value.

### HasRemoveLabels

`func (o *UpdateEmailRequest) HasRemoveLabels() bool`

HasRemoveLabels returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


