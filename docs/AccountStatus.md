# AccountStatus

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Provider** | **string** | Provider id (e.g. &#x60;native-notes&#x60;, &#x60;notion&#x60;, &#x60;google-keep&#x60;). | 
**AccountId** | **string** | Connected-account row id. | 
**AccountName** | Pointer to **string** | Human-readable label for the account, when available. | [optional] 
**Status** | **string** | - &#x60;ok&#x60; — provider call returned without error. - &#x60;error&#x60; — provider call failed; details in &#x60;error&#x60;. - &#x60;skipped&#x60; — connection was filtered out before the provider   call ran. Reserved; not currently emitted by the runtime.  | 
**Error** | Pointer to [**AccountError**](AccountError.md) |  | [optional] 
**NextPageToken** | Pointer to **string** | Provider-specific cursor for the next page, if any. | [optional] 

## Methods

### NewAccountStatus

`func NewAccountStatus(provider string, accountId string, status string, ) *AccountStatus`

NewAccountStatus instantiates a new AccountStatus object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAccountStatusWithDefaults

`func NewAccountStatusWithDefaults() *AccountStatus`

NewAccountStatusWithDefaults instantiates a new AccountStatus object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProvider

`func (o *AccountStatus) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *AccountStatus) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *AccountStatus) SetProvider(v string)`

SetProvider sets Provider field to given value.


### GetAccountId

`func (o *AccountStatus) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *AccountStatus) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *AccountStatus) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.


### GetAccountName

`func (o *AccountStatus) GetAccountName() string`

GetAccountName returns the AccountName field if non-nil, zero value otherwise.

### GetAccountNameOk

`func (o *AccountStatus) GetAccountNameOk() (*string, bool)`

GetAccountNameOk returns a tuple with the AccountName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountName

`func (o *AccountStatus) SetAccountName(v string)`

SetAccountName sets AccountName field to given value.

### HasAccountName

`func (o *AccountStatus) HasAccountName() bool`

HasAccountName returns a boolean if a field has been set.

### GetStatus

`func (o *AccountStatus) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *AccountStatus) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *AccountStatus) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetError

`func (o *AccountStatus) GetError() AccountError`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *AccountStatus) GetErrorOk() (*AccountError, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *AccountStatus) SetError(v AccountError)`

SetError sets Error field to given value.

### HasError

`func (o *AccountStatus) HasError() bool`

HasError returns a boolean if a field has been set.

### GetNextPageToken

`func (o *AccountStatus) GetNextPageToken() string`

GetNextPageToken returns the NextPageToken field if non-nil, zero value otherwise.

### GetNextPageTokenOk

`func (o *AccountStatus) GetNextPageTokenOk() (*string, bool)`

GetNextPageTokenOk returns a tuple with the NextPageToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPageToken

`func (o *AccountStatus) SetNextPageToken(v string)`

SetNextPageToken sets NextPageToken field to given value.

### HasNextPageToken

`func (o *AccountStatus) HasNextPageToken() bool`

HasNextPageToken returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


