# ConnectionAccountListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Connections** | Pointer to **[]map[string]interface{}** |  | [optional] 
**UserId** | Pointer to **string** |  | [optional] 
**Accounts** | Pointer to **[]map[string]interface{}** |  | [optional] 

## Methods

### NewConnectionAccountListResponse

`func NewConnectionAccountListResponse() *ConnectionAccountListResponse`

NewConnectionAccountListResponse instantiates a new ConnectionAccountListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewConnectionAccountListResponseWithDefaults

`func NewConnectionAccountListResponseWithDefaults() *ConnectionAccountListResponse`

NewConnectionAccountListResponseWithDefaults instantiates a new ConnectionAccountListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetConnections

`func (o *ConnectionAccountListResponse) GetConnections() []map[string]interface{}`

GetConnections returns the Connections field if non-nil, zero value otherwise.

### GetConnectionsOk

`func (o *ConnectionAccountListResponse) GetConnectionsOk() (*[]map[string]interface{}, bool)`

GetConnectionsOk returns a tuple with the Connections field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConnections

`func (o *ConnectionAccountListResponse) SetConnections(v []map[string]interface{})`

SetConnections sets Connections field to given value.

### HasConnections

`func (o *ConnectionAccountListResponse) HasConnections() bool`

HasConnections returns a boolean if a field has been set.

### SetConnectionsNil

`func (o *ConnectionAccountListResponse) SetConnectionsNil(b bool)`

 SetConnectionsNil sets the value for Connections to be an explicit nil

### UnsetConnections
`func (o *ConnectionAccountListResponse) UnsetConnections()`

UnsetConnections ensures that no value is present for Connections, not even an explicit nil
### GetUserId

`func (o *ConnectionAccountListResponse) GetUserId() string`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *ConnectionAccountListResponse) GetUserIdOk() (*string, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *ConnectionAccountListResponse) SetUserId(v string)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *ConnectionAccountListResponse) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetAccounts

`func (o *ConnectionAccountListResponse) GetAccounts() []map[string]interface{}`

GetAccounts returns the Accounts field if non-nil, zero value otherwise.

### GetAccountsOk

`func (o *ConnectionAccountListResponse) GetAccountsOk() (*[]map[string]interface{}, bool)`

GetAccountsOk returns a tuple with the Accounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccounts

`func (o *ConnectionAccountListResponse) SetAccounts(v []map[string]interface{})`

SetAccounts sets Accounts field to given value.

### HasAccounts

`func (o *ConnectionAccountListResponse) HasAccounts() bool`

HasAccounts returns a boolean if a field has been set.

### SetAccountsNil

`func (o *ConnectionAccountListResponse) SetAccountsNil(b bool)`

 SetAccountsNil sets the value for Accounts to be an explicit nil

### UnsetAccounts
`func (o *ConnectionAccountListResponse) UnsetAccounts()`

UnsetAccounts ensures that no value is present for Accounts, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


