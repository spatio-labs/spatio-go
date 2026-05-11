# AccountListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccountsByPlatform** | Pointer to **map[string]interface{}** |  | [optional] 
**TotalAccounts** | Pointer to **int32** |  | [optional] 
**Accounts** | Pointer to **[]map[string]interface{}** |  | [optional] 

## Methods

### NewAccountListResponse

`func NewAccountListResponse() *AccountListResponse`

NewAccountListResponse instantiates a new AccountListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAccountListResponseWithDefaults

`func NewAccountListResponseWithDefaults() *AccountListResponse`

NewAccountListResponseWithDefaults instantiates a new AccountListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccountsByPlatform

`func (o *AccountListResponse) GetAccountsByPlatform() map[string]interface{}`

GetAccountsByPlatform returns the AccountsByPlatform field if non-nil, zero value otherwise.

### GetAccountsByPlatformOk

`func (o *AccountListResponse) GetAccountsByPlatformOk() (*map[string]interface{}, bool)`

GetAccountsByPlatformOk returns a tuple with the AccountsByPlatform field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountsByPlatform

`func (o *AccountListResponse) SetAccountsByPlatform(v map[string]interface{})`

SetAccountsByPlatform sets AccountsByPlatform field to given value.

### HasAccountsByPlatform

`func (o *AccountListResponse) HasAccountsByPlatform() bool`

HasAccountsByPlatform returns a boolean if a field has been set.

### GetTotalAccounts

`func (o *AccountListResponse) GetTotalAccounts() int32`

GetTotalAccounts returns the TotalAccounts field if non-nil, zero value otherwise.

### GetTotalAccountsOk

`func (o *AccountListResponse) GetTotalAccountsOk() (*int32, bool)`

GetTotalAccountsOk returns a tuple with the TotalAccounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalAccounts

`func (o *AccountListResponse) SetTotalAccounts(v int32)`

SetTotalAccounts sets TotalAccounts field to given value.

### HasTotalAccounts

`func (o *AccountListResponse) HasTotalAccounts() bool`

HasTotalAccounts returns a boolean if a field has been set.

### GetAccounts

`func (o *AccountListResponse) GetAccounts() []map[string]interface{}`

GetAccounts returns the Accounts field if non-nil, zero value otherwise.

### GetAccountsOk

`func (o *AccountListResponse) GetAccountsOk() (*[]map[string]interface{}, bool)`

GetAccountsOk returns a tuple with the Accounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccounts

`func (o *AccountListResponse) SetAccounts(v []map[string]interface{})`

SetAccounts sets Accounts field to given value.

### HasAccounts

`func (o *AccountListResponse) HasAccounts() bool`

HasAccounts returns a boolean if a field has been set.

### SetAccountsNil

`func (o *AccountListResponse) SetAccountsNil(b bool)`

 SetAccountsNil sets the value for Accounts to be an explicit nil

### UnsetAccounts
`func (o *AccountListResponse) UnsetAccounts()`

UnsetAccounts ensures that no value is present for Accounts, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


