# SearchEmailsResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Emails** | Pointer to [**[]Email**](Email.md) | &#x60;null&#x60; when there are no results (Go nil-slice serialization). Treat as equivalent to an empty array.  | [optional] 
**Total** | **int32** |  | 
**NextPageToken** | Pointer to **string** |  | [optional] 
**Provider** | **string** |  | 

## Methods

### NewSearchEmailsResponse

`func NewSearchEmailsResponse(total int32, provider string, ) *SearchEmailsResponse`

NewSearchEmailsResponse instantiates a new SearchEmailsResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSearchEmailsResponseWithDefaults

`func NewSearchEmailsResponseWithDefaults() *SearchEmailsResponse`

NewSearchEmailsResponseWithDefaults instantiates a new SearchEmailsResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmails

`func (o *SearchEmailsResponse) GetEmails() []Email`

GetEmails returns the Emails field if non-nil, zero value otherwise.

### GetEmailsOk

`func (o *SearchEmailsResponse) GetEmailsOk() (*[]Email, bool)`

GetEmailsOk returns a tuple with the Emails field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmails

`func (o *SearchEmailsResponse) SetEmails(v []Email)`

SetEmails sets Emails field to given value.

### HasEmails

`func (o *SearchEmailsResponse) HasEmails() bool`

HasEmails returns a boolean if a field has been set.

### SetEmailsNil

`func (o *SearchEmailsResponse) SetEmailsNil(b bool)`

 SetEmailsNil sets the value for Emails to be an explicit nil

### UnsetEmails
`func (o *SearchEmailsResponse) UnsetEmails()`

UnsetEmails ensures that no value is present for Emails, not even an explicit nil
### GetTotal

`func (o *SearchEmailsResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *SearchEmailsResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *SearchEmailsResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.


### GetNextPageToken

`func (o *SearchEmailsResponse) GetNextPageToken() string`

GetNextPageToken returns the NextPageToken field if non-nil, zero value otherwise.

### GetNextPageTokenOk

`func (o *SearchEmailsResponse) GetNextPageTokenOk() (*string, bool)`

GetNextPageTokenOk returns a tuple with the NextPageToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPageToken

`func (o *SearchEmailsResponse) SetNextPageToken(v string)`

SetNextPageToken sets NextPageToken field to given value.

### HasNextPageToken

`func (o *SearchEmailsResponse) HasNextPageToken() bool`

HasNextPageToken returns a boolean if a field has been set.

### GetProvider

`func (o *SearchEmailsResponse) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *SearchEmailsResponse) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *SearchEmailsResponse) SetProvider(v string)`

SetProvider sets Provider field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


