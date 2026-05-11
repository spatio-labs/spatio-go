# DisconnectConnectionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ConnectionId** | **string** |  | 
**AccountId** | Pointer to **string** |  | [optional] 

## Methods

### NewDisconnectConnectionRequest

`func NewDisconnectConnectionRequest(connectionId string, ) *DisconnectConnectionRequest`

NewDisconnectConnectionRequest instantiates a new DisconnectConnectionRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDisconnectConnectionRequestWithDefaults

`func NewDisconnectConnectionRequestWithDefaults() *DisconnectConnectionRequest`

NewDisconnectConnectionRequestWithDefaults instantiates a new DisconnectConnectionRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetConnectionId

`func (o *DisconnectConnectionRequest) GetConnectionId() string`

GetConnectionId returns the ConnectionId field if non-nil, zero value otherwise.

### GetConnectionIdOk

`func (o *DisconnectConnectionRequest) GetConnectionIdOk() (*string, bool)`

GetConnectionIdOk returns a tuple with the ConnectionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConnectionId

`func (o *DisconnectConnectionRequest) SetConnectionId(v string)`

SetConnectionId sets ConnectionId field to given value.


### GetAccountId

`func (o *DisconnectConnectionRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *DisconnectConnectionRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *DisconnectConnectionRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *DisconnectConnectionRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


