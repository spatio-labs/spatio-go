# UpdateEventRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccountId** | **string** |  | 
**Updates** | **map[string]interface{}** |  | 
**SendUpdates** | Pointer to **string** |  | [optional] 

## Methods

### NewUpdateEventRequest

`func NewUpdateEventRequest(accountId string, updates map[string]interface{}, ) *UpdateEventRequest`

NewUpdateEventRequest instantiates a new UpdateEventRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateEventRequestWithDefaults

`func NewUpdateEventRequestWithDefaults() *UpdateEventRequest`

NewUpdateEventRequestWithDefaults instantiates a new UpdateEventRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccountId

`func (o *UpdateEventRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *UpdateEventRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *UpdateEventRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.


### GetUpdates

`func (o *UpdateEventRequest) GetUpdates() map[string]interface{}`

GetUpdates returns the Updates field if non-nil, zero value otherwise.

### GetUpdatesOk

`func (o *UpdateEventRequest) GetUpdatesOk() (*map[string]interface{}, bool)`

GetUpdatesOk returns a tuple with the Updates field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdates

`func (o *UpdateEventRequest) SetUpdates(v map[string]interface{})`

SetUpdates sets Updates field to given value.


### GetSendUpdates

`func (o *UpdateEventRequest) GetSendUpdates() string`

GetSendUpdates returns the SendUpdates field if non-nil, zero value otherwise.

### GetSendUpdatesOk

`func (o *UpdateEventRequest) GetSendUpdatesOk() (*string, bool)`

GetSendUpdatesOk returns a tuple with the SendUpdates field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSendUpdates

`func (o *UpdateEventRequest) SetSendUpdates(v string)`

SetSendUpdates sets SendUpdates field to given value.

### HasSendUpdates

`func (o *UpdateEventRequest) HasSendUpdates() bool`

HasSendUpdates returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


