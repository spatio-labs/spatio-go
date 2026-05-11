# RefreshConnectionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ConnectionId** | **string** |  | 
**AccountId** | Pointer to **string** |  | [optional] 

## Methods

### NewRefreshConnectionRequest

`func NewRefreshConnectionRequest(connectionId string, ) *RefreshConnectionRequest`

NewRefreshConnectionRequest instantiates a new RefreshConnectionRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRefreshConnectionRequestWithDefaults

`func NewRefreshConnectionRequestWithDefaults() *RefreshConnectionRequest`

NewRefreshConnectionRequestWithDefaults instantiates a new RefreshConnectionRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetConnectionId

`func (o *RefreshConnectionRequest) GetConnectionId() string`

GetConnectionId returns the ConnectionId field if non-nil, zero value otherwise.

### GetConnectionIdOk

`func (o *RefreshConnectionRequest) GetConnectionIdOk() (*string, bool)`

GetConnectionIdOk returns a tuple with the ConnectionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConnectionId

`func (o *RefreshConnectionRequest) SetConnectionId(v string)`

SetConnectionId sets ConnectionId field to given value.


### GetAccountId

`func (o *RefreshConnectionRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *RefreshConnectionRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *RefreshConnectionRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *RefreshConnectionRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


