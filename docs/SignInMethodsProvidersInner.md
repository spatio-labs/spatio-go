# SignInMethodsProvidersInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Provider** | **string** | OAuth IdP: &#x60;GOOGLE&#x60;, &#x60;GITHUB&#x60;, etc. | 
**AccountEmail** | Pointer to **string** |  | [optional] 
**LinkedAt** | Pointer to **time.Time** |  | [optional] 
**LastUsedAt** | Pointer to **NullableTime** |  | [optional] 

## Methods

### NewSignInMethodsProvidersInner

`func NewSignInMethodsProvidersInner(provider string, ) *SignInMethodsProvidersInner`

NewSignInMethodsProvidersInner instantiates a new SignInMethodsProvidersInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSignInMethodsProvidersInnerWithDefaults

`func NewSignInMethodsProvidersInnerWithDefaults() *SignInMethodsProvidersInner`

NewSignInMethodsProvidersInnerWithDefaults instantiates a new SignInMethodsProvidersInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProvider

`func (o *SignInMethodsProvidersInner) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *SignInMethodsProvidersInner) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *SignInMethodsProvidersInner) SetProvider(v string)`

SetProvider sets Provider field to given value.


### GetAccountEmail

`func (o *SignInMethodsProvidersInner) GetAccountEmail() string`

GetAccountEmail returns the AccountEmail field if non-nil, zero value otherwise.

### GetAccountEmailOk

`func (o *SignInMethodsProvidersInner) GetAccountEmailOk() (*string, bool)`

GetAccountEmailOk returns a tuple with the AccountEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountEmail

`func (o *SignInMethodsProvidersInner) SetAccountEmail(v string)`

SetAccountEmail sets AccountEmail field to given value.

### HasAccountEmail

`func (o *SignInMethodsProvidersInner) HasAccountEmail() bool`

HasAccountEmail returns a boolean if a field has been set.

### GetLinkedAt

`func (o *SignInMethodsProvidersInner) GetLinkedAt() time.Time`

GetLinkedAt returns the LinkedAt field if non-nil, zero value otherwise.

### GetLinkedAtOk

`func (o *SignInMethodsProvidersInner) GetLinkedAtOk() (*time.Time, bool)`

GetLinkedAtOk returns a tuple with the LinkedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLinkedAt

`func (o *SignInMethodsProvidersInner) SetLinkedAt(v time.Time)`

SetLinkedAt sets LinkedAt field to given value.

### HasLinkedAt

`func (o *SignInMethodsProvidersInner) HasLinkedAt() bool`

HasLinkedAt returns a boolean if a field has been set.

### GetLastUsedAt

`func (o *SignInMethodsProvidersInner) GetLastUsedAt() time.Time`

GetLastUsedAt returns the LastUsedAt field if non-nil, zero value otherwise.

### GetLastUsedAtOk

`func (o *SignInMethodsProvidersInner) GetLastUsedAtOk() (*time.Time, bool)`

GetLastUsedAtOk returns a tuple with the LastUsedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastUsedAt

`func (o *SignInMethodsProvidersInner) SetLastUsedAt(v time.Time)`

SetLastUsedAt sets LastUsedAt field to given value.

### HasLastUsedAt

`func (o *SignInMethodsProvidersInner) HasLastUsedAt() bool`

HasLastUsedAt returns a boolean if a field has been set.

### SetLastUsedAtNil

`func (o *SignInMethodsProvidersInner) SetLastUsedAtNil(b bool)`

 SetLastUsedAtNil sets the value for LastUsedAt to be an explicit nil

### UnsetLastUsedAt
`func (o *SignInMethodsProvidersInner) UnsetLastUsedAt()`

UnsetLastUsedAt ensures that no value is present for LastUsedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


