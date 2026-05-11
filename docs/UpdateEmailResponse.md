# UpdateEmailResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Email** | [**Email**](Email.md) |  | 
**Provider** | **string** |  | 

## Methods

### NewUpdateEmailResponse

`func NewUpdateEmailResponse(email Email, provider string, ) *UpdateEmailResponse`

NewUpdateEmailResponse instantiates a new UpdateEmailResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateEmailResponseWithDefaults

`func NewUpdateEmailResponseWithDefaults() *UpdateEmailResponse`

NewUpdateEmailResponseWithDefaults instantiates a new UpdateEmailResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmail

`func (o *UpdateEmailResponse) GetEmail() Email`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *UpdateEmailResponse) GetEmailOk() (*Email, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *UpdateEmailResponse) SetEmail(v Email)`

SetEmail sets Email field to given value.


### GetProvider

`func (o *UpdateEmailResponse) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *UpdateEmailResponse) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *UpdateEmailResponse) SetProvider(v string)`

SetProvider sets Provider field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


