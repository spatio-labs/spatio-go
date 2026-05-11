# SignInMethods

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Email** | **string** |  | 
**HasPassword** | **bool** |  | 
**Providers** | Pointer to [**[]SignInMethodsProvidersInner**](SignInMethodsProvidersInner.md) |  | [optional] 

## Methods

### NewSignInMethods

`func NewSignInMethods(email string, hasPassword bool, ) *SignInMethods`

NewSignInMethods instantiates a new SignInMethods object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSignInMethodsWithDefaults

`func NewSignInMethodsWithDefaults() *SignInMethods`

NewSignInMethodsWithDefaults instantiates a new SignInMethods object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmail

`func (o *SignInMethods) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *SignInMethods) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *SignInMethods) SetEmail(v string)`

SetEmail sets Email field to given value.


### GetHasPassword

`func (o *SignInMethods) GetHasPassword() bool`

GetHasPassword returns the HasPassword field if non-nil, zero value otherwise.

### GetHasPasswordOk

`func (o *SignInMethods) GetHasPasswordOk() (*bool, bool)`

GetHasPasswordOk returns a tuple with the HasPassword field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasPassword

`func (o *SignInMethods) SetHasPassword(v bool)`

SetHasPassword sets HasPassword field to given value.


### GetProviders

`func (o *SignInMethods) GetProviders() []SignInMethodsProvidersInner`

GetProviders returns the Providers field if non-nil, zero value otherwise.

### GetProvidersOk

`func (o *SignInMethods) GetProvidersOk() (*[]SignInMethodsProvidersInner, bool)`

GetProvidersOk returns a tuple with the Providers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProviders

`func (o *SignInMethods) SetProviders(v []SignInMethodsProvidersInner)`

SetProviders sets Providers field to given value.

### HasProviders

`func (o *SignInMethods) HasProviders() bool`

HasProviders returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


