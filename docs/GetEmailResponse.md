# GetEmailResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Email** | [**Email**](Email.md) |  | 
**Provider** | **string** |  | 

## Methods

### NewGetEmailResponse

`func NewGetEmailResponse(email Email, provider string, ) *GetEmailResponse`

NewGetEmailResponse instantiates a new GetEmailResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetEmailResponseWithDefaults

`func NewGetEmailResponseWithDefaults() *GetEmailResponse`

NewGetEmailResponseWithDefaults instantiates a new GetEmailResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmail

`func (o *GetEmailResponse) GetEmail() Email`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *GetEmailResponse) GetEmailOk() (*Email, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *GetEmailResponse) SetEmail(v Email)`

SetEmail sets Email field to given value.


### GetProvider

`func (o *GetEmailResponse) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *GetEmailResponse) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *GetEmailResponse) SetProvider(v string)`

SetProvider sets Provider field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


