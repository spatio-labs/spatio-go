# ConnectionListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Connections** | [**[]SpatioConnection**](SpatioConnection.md) |  | 
**Categories** | Pointer to **[]string** |  | [optional] 

## Methods

### NewConnectionListResponse

`func NewConnectionListResponse(connections []SpatioConnection, ) *ConnectionListResponse`

NewConnectionListResponse instantiates a new ConnectionListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewConnectionListResponseWithDefaults

`func NewConnectionListResponseWithDefaults() *ConnectionListResponse`

NewConnectionListResponseWithDefaults instantiates a new ConnectionListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetConnections

`func (o *ConnectionListResponse) GetConnections() []SpatioConnection`

GetConnections returns the Connections field if non-nil, zero value otherwise.

### GetConnectionsOk

`func (o *ConnectionListResponse) GetConnectionsOk() (*[]SpatioConnection, bool)`

GetConnectionsOk returns a tuple with the Connections field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConnections

`func (o *ConnectionListResponse) SetConnections(v []SpatioConnection)`

SetConnections sets Connections field to given value.


### GetCategories

`func (o *ConnectionListResponse) GetCategories() []string`

GetCategories returns the Categories field if non-nil, zero value otherwise.

### GetCategoriesOk

`func (o *ConnectionListResponse) GetCategoriesOk() (*[]string, bool)`

GetCategoriesOk returns a tuple with the Categories field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategories

`func (o *ConnectionListResponse) SetCategories(v []string)`

SetCategories sets Categories field to given value.

### HasCategories

`func (o *ConnectionListResponse) HasCategories() bool`

HasCategories returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


